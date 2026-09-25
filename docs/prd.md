# 📄 Product Requirements Document (PRD) - ClutchBR

## 1. Visão Geral e Objetivo

O **ClutchBR** é uma aplicação web voltada para a comunidade brasileira de **Counter-Strike 2**, reunindo informações sobre jogadores, equipes e partidas do cenário competitivo.

O objetivo é facilitar o acesso a essas informações em um único lugar e oferecer um espaço simples para que usuários possam compartilhar conteúdos e interagir com a comunidade.

## 2. Atores do Sistema

- **Visitante:** Usuário não autenticado que pode visualizar jogadores, equipes e partidas.
- **Usuário:** Pessoa autenticada que pode visualizar as informações do cenário competitivo, criar publicações e realizar comentários.
- **Sistema:** Responsável por buscar os dados competitivos através da API pública e gerenciar os dados da comunidade através da API própria.

## 3. Histórias de Usuário e Escopo

Abaixo estão as funcionalidades principais do MVP (Minimum Viable Product).

### 🎮 Épico 1: Cenário Competitivo

- **US01 - Visualizar Jogadores:** Como um Visitante, quero visualizar jogadores profissionais de Counter-Strike para conhecer seus dados e equipes.
  - _Critérios de Aceitação:_ O sistema deve apresentar o nome do jogador, sua equipe e as informações disponíveis pela API.

- **US02 - Visualizar Equipes:** Como um Visitante, quero visualizar equipes profissionais para conhecer seus jogadores e informações.
  - _Critérios de Aceitação:_ O sistema deve apresentar o nome da equipe e os jogadores relacionados quando essas informações estiverem disponíveis.

- **US03 - Visualizar Partidas:** Como um Visitante, quero visualizar partidas de Counter-Strike para acompanhar os confrontos do cenário competitivo.
  - _Critérios de Aceitação:_ O sistema deve apresentar as equipes participantes, data e resultado da partida quando disponível.

### 👤 Épico 2: Conta de Usuário

- **US04 - Criar Conta:** Como um Visitante, quero criar uma conta para participar da comunidade.
  - _Critérios de Aceitação:_ O usuário deve preencher os dados obrigatórios para criar sua conta.

- **US05 - Login:** Como um Usuário, quero realizar login para acessar as funcionalidades da comunidade.
  - _Critérios de Aceitação:_ O sistema deve validar os dados informados antes de permitir o acesso.

### 💬 Épico 3: Comunidade

- **US06 - Criar Publicação:** Como um Usuário, quero criar uma publicação para compartilhar conteúdos e opiniões sobre Counter-Strike.
  - _Critérios de Aceitação:_ O usuário deve estar autenticado e informar o conteúdo da publicação.

- **US07 - Comentar Publicação:** Como um Usuário, quero comentar nas publicações para participar das discussões da comunidade.
  - _Critérios de Aceitação:_ O usuário deve estar autenticado e o comentário deve ficar relacionado à publicação.

## 4. MVP

O MVP do **ClutchBR** será composto por:

- Página inicial;
- Visualização de jogadores;
- Visualização de equipes;
- Visualização de partidas;
- Cadastro de usuários;
- Login;
- Publicações;
- Comentários;
- Layout responsivo;
- Integração com a API pública de Counter-Strike;
- API própria simulada com JSON Server.

Funcionalidades como ranking, campeonatos, notícias, favoritos, inventários, skins e outras funcionalidades avançadas poderão ser adicionadas em versões futuras.
