# 🛠️ Especificação Técnica (Tech Spec) - ClutchBR

Este documento detalha a arquitetura técnica, o modelo de dados e os contratos de API necessários para o funcionamento do sistema ClutchBR.

## 1. Modelo de Dados (Diagrama ER)

Abaixo está o Diagrama Entidade-Relacionamento (DER) que representa a estrutura do banco de dados simulado (`db.json`) e como as informações da comunidade se conectam.

Os dados de jogadores, equipes e partidas não serão armazenados no `db.json`, pois serão obtidos através da API pública do Counter-Strike.

```mermaid
erDiagram

USUARIO ||--o{ PUBLICACAO : "cria"
USUARIO ||--o{ COMENTARIO : "realiza"
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
