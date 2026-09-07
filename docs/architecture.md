# 🛠️ Especificação Técnica (Tech Spec) - ClutchBR

Este documento detalha a arquitetura técnica, o modelo de dados e os contratos de API necessários para o funcionamento do sistema ClutchBR.

## 1. Modelo de Dados (Diagrama ER)

Abaixo está o Diagrama Entidade-Relacionamento (DER) que representa a estrutura do banco de dados simulado (`db.json`) e como as informações se conectam.

```mermaid
erDiagram

USUARIO ||--o{ PUBLICACAO : "cria"
USUARIO ||--o{ COMENTARIO : "realiza"
USUARIO ||--o{ FAVORITO : "possui"
PUBLICACAO ||--o{ COMENTARIO : "recebe"

USUARIO {
    string id PK "Gerado pelo JSON Server"
    string nome
    string email
    string senha
}

PUBLICACAO {
    string id PK
    string usuarioId FK
    string titulo
    string conteudo
    string data
}

COMENTARIO {
    string id PK
    string usuarioId FK
    string publicacaoId FK
    string conteudo
    string data
}

FAVORITO {
    string id PK
    string usuarioId FK
    string tipo "JOGADOR ou EQUIPE"
    string referenciaId
}
```

Os dados relacionados ao cenário competitivo, como jogadores, equipes, partidas e rankings, serão obtidos através da API pública do Counter-Strike.

## 2. Dicionário de Dados

Breve explicação das principais entidades:

- **Usuários:** Responsável por armazenar os dados necessários para autenticação e identificação dos usuários da comunidade.
  - `id`: Identificador único do usuário.
  - `nome`: Nome utilizado pelo usuário na plataforma.
  - `email`: E-mail utilizado para acesso à conta.
  - `senha`: Senha utilizada na autenticação.

- **Publicações:** Armazena os conteúdos criados pelos usuários na área da comunidade.
  - `id`: Identificador único da publicação.
  - `usuarioId`: Identifica o usuário responsável pela publicação.
  - `titulo`: Título da publicação.
  - `conteudo`: Texto da publicação.
  - `data`: Data em que a publicação foi criada.

- **Comentários:** Armazena os comentários realizados nas publicações.
  - `id`: Identificador único do comentário.
  - `usuarioId`: Usuário que realizou o comentário.
  - `publicacaoId`: Publicação relacionada ao comentário.
  - `conteudo`: Texto do comentário.
  - `data`: Data em que o comentário foi realizado.

- **Favoritos:** Armazena jogadores e equipes favoritados pelos usuários.
  - `id`: Identificador único do favorito.
  - `usuarioId`: Usuário que adicionou o favorito.
  - `tipo`: Define se o favorito é um jogador ou uma equipe.
  - `referenciaId`: Identificador do jogador ou equipe favoritado.


## 3. Tecnologias

As principais tecnologias previstas para o desenvolvimento do ClutchBR são:

- **HTML5** - Estrutura das páginas.
- **CSS3** - Estilização da aplicação.
- **Bootstrap 5** - Framework CSS utilizado para componentes e responsividade.
- **Sass (SCSS)** - Organização e gerenciamento dos estilos.
- **JavaScript** - Interações e funcionalidades da aplicação.
- **JSON Server** - Simulação da API própria do sistema.
- **CS API** - Fornecimento dos dados do cenário competitivo.
