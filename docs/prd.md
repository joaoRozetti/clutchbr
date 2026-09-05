# Product Requirements Document (PRD) — ClutchBR

## 1. Visão do Produto

O **ClutchBR** é uma plataforma web voltada à comunidade brasileira de **Counter-Strike**, com foco no cenário competitivo e na centralização de informações sobre jogadores, equipes, partidas, campeonatos e notícias.

A aplicação tem como objetivo proporcionar aos fãs de Counter-Strike um ambiente único para acompanhar o cenário competitivo, consultar informações sobre jogadores e equipes e interagir com outros membros da comunidade.

O projeto terá como foco principal o **Counter-Strike 2 (CS2)**, mantendo também uma relação histórica com o Counter-Strike: Global Offensive (CS:GO).

Os dados relacionados ao cenário competitivo serão obtidos por meio da **CS API**, enquanto informações próprias da aplicação, como conteúdos da comunidade, poderão ser simuladas por meio de uma API Fake utilizando **JSON Server**.

---

## 2. Problema

As informações relacionadas ao cenário competitivo de Counter-Strike estão distribuídas entre diferentes plataformas, sites e comunidades.

Um usuário interessado no cenário brasileiro pode precisar acessar diferentes fontes para consultar:

- Notícias;
- Partidas;
- Campeonatos;
- Equipes;
- Jogadores;
- Estatísticas;
- Rankings;
- Conteúdos da comunidade.

O ClutchBR busca solucionar esse problema centralizando essas informações em uma única plataforma, com uma interface direcionada ao público brasileiro.

---

## 3. Objetivos

### 3.1 Objetivo Geral

Desenvolver uma plataforma web responsiva capaz de centralizar informações sobre o cenário competitivo de Counter-Strike e oferecer recursos voltados à comunidade brasileira.

### 3.2 Objetivos Específicos

- Disponibilizar informações sobre partidas e campeonatos;
- Apresentar informações sobre equipes profissionais;
- Apresentar perfis de jogadores profissionais;
- Exibir estatísticas disponibilizadas pela API;
- Permitir a pesquisa de jogadores e equipes;
- Disponibilizar notícias relacionadas ao cenário;
- Criar uma área voltada à comunidade;
- Permitir a publicação e visualização de discussões;
- Permitir comentários nas publicações;
- Permitir que usuários salvem conteúdos como favoritos;
- Desenvolver uma interface responsiva para dispositivos móveis e desktop;
- Consumir dados de uma API pública relacionada ao Counter-Strike;
- Utilizar uma API Fake para simular funcionalidades que necessitem de persistência própria.

---

# 4. Público-Alvo

O ClutchBR será direcionado principalmente para usuários brasileiros interessados em Counter-Strike.

### 4.1 Jogadores

Pessoas que jogam Counter-Strike e desejam acompanhar o cenário competitivo, jogadores profissionais, equipes e estatísticas.

### 4.2 Fãs de Esports

Usuários que acompanham campeonatos profissionais e desejam consultar partidas, resultados, equipes e jogadores.

### 4.3 Comunidade Brasileira

Pessoas interessadas em discutir partidas, equipes, jogadores e acontecimentos relacionados ao cenário brasileiro de Counter-Strike.

### 4.4 Usuários Casuais

Pessoas que possuem interesse no jogo, mas não acompanham constantemente o cenário competitivo e desejam encontrar informações de forma simples e organizada.

---

# 5. Atores do Sistema

## 5.1 Visitante

Usuário que acessa o ClutchBR sem realizar login.

Pode:

- Visualizar notícias;
- Consultar partidas;
- Visualizar campeonatos;
- Consultar equipes;
- Consultar jogadores;
- Visualizar estatísticas;
- Pesquisar informações;
- Visualizar conteúdos públicos da comunidade.

## 5.2 Usuário

Usuário cadastrado na plataforma.

Além das funcionalidades disponíveis ao visitante, poderá:

- Criar publicações;
- Comentar em publicações;
- Favoritar conteúdos;
- Gerenciar seu perfil;
- Participar das discussões da comunidade.

## 5.3 Administrador

Responsável pela administração dos conteúdos e da comunidade.

Poderá:

- Gerenciar publicações;
- Gerenciar comentários;
- Remover conteúdos inadequados;
- Gerenciar usuários;
- Administrar conteúdos da plataforma.

---

# 6. Escopo do Projeto

## 6.1 Dentro do Escopo

O projeto contemplará:

- Página inicial;
- Notícias;
- Partidas;
- Campeonatos;
- Equipes;
- Jogadores;
- Estatísticas;
- Rankings;
- Pesquisa;
- Filtros;
- Área da comunidade;
- Publicações;
- Comentários;
- Favoritos;
- Perfil de usuário;
- Integração com API pública;
- API Fake para dados próprios da aplicação;
- Interface responsiva;
- Design System próprio.

## 6.2 Fora do Escopo

Não fazem parte do escopo inicial:

- Sistema de matchmaking;
- Servidores próprios de Counter-Strike;
- Venda ou compra real de skins;
- Transações financeiras;
- Sistema de apostas;
- Reprodução de partidas ao vivo;
- Sistema de transmissão de campeonatos;
- Desenvolvimento de um aplicativo mobile nativo;
- Integração com sistemas oficiais da Steam para autenticação.

Funcionalidades adicionais poderão ser consideradas futuramente, dependendo da viabilidade técnica.

---

# 7. Funcionalidades

## 7.1 Página Inicial

A página inicial deverá apresentar um resumo das principais informações disponíveis no ClutchBR.

Deverá apresentar:

- Notícias em destaque;
- Últimas notícias;
- Próximas partidas;
- Resultados recentes;
- Principais equipes;
- Informações relevantes do cenário competitivo.

---

## 7.2 Notícias

O usuário poderá visualizar notícias relacionadas ao universo de Counter-Strike.

Cada notícia poderá apresentar:

- Título;
- Imagem;
- Resumo;
- Data de publicação;
- Categoria;
- Conteúdo completo.

---

## 7.3 Partidas

O sistema deverá apresentar partidas do cenário competitivo.

Cada partida poderá apresentar:

- Equipes participantes;
- Data;
- Horário;
- Campeonato;
- Status da partida;
- Resultado, quando disponível;
- Mapas, quando disponibilizados pela API.

---

## 7.4 Campeonatos

O usuário poderá consultar campeonatos relacionados ao cenário competitivo.

As informações poderão incluir:

- Nome do campeonato;
- Status;
- Data de início;
- Data de término;
- Equipes participantes;
- Partidas;
- Resultados.

---

## 7.5 Equipes

O sistema deverá disponibilizar uma página para consulta das equipes profissionais.

Cada equipe poderá apresentar:

- Nome;
- Logo;
- País;
- Jogadores;
- Ranking;
- Partidas;
- Resultados;
- Estatísticas disponíveis.

---

## 7.6 Jogadores

O sistema deverá disponibilizar perfis de jogadores profissionais.

O perfil poderá apresentar:

- Nome;
- Nickname;
- Nacionalidade;
- Equipe atual;
- Histórico de equipes;
- Estatísticas;
- Partidas;
- Informações competitivas disponíveis.

---

## 7.7 Inventário de Jogadores

O projeto poderá apresentar informações sobre os inventários públicos de jogadores profissionais.

Quando houver uma API ou serviço compatível e tecnicamente viável, o sistema poderá apresentar:

- Skins;
- Facas;
- Luvas;
- Adesivos;
- Outros itens disponíveis;
- Informações básicas dos itens.

Essa funcionalidade dependerá da disponibilidade, estabilidade e permissões dos serviços utilizados.

---

## 7.8 Pesquisa

O usuário poderá pesquisar informações dentro da plataforma.

A pesquisa poderá retornar:

- Jogadores;
- Equipes;
- Campeonatos;
- Notícias.

---

## 7.9 Filtros

O sistema deverá disponibilizar filtros para facilitar a localização das informações.

Os filtros poderão incluir:

- Equipe;
- Jogador;
- Campeonato;
- Data;
- Status da partida;
- País.

---

## 7.10 Comunidade

O ClutchBR contará com uma área destinada à interação entre os usuários.

Os usuários cadastrados poderão criar publicações relacionadas ao Counter-Strike.

As publicações poderão conter:

- Título;
- Texto;
- Data;
- Autor;
- Categoria;
- Comentários.

---

## 7.11 Comentários

Usuários autenticados poderão comentar nas publicações da comunidade.

Os comentários deverão apresentar:

- Autor;
- Conteúdo;
- Data de publicação.

---

## 7.12 Favoritos

Usuários autenticados poderão favoritar conteúdos da plataforma.

Inicialmente, poderão ser favoritados:

- Notícias;
- Jogadores;
- Equipes;
- Campeonatos.

---

## 7.13 Perfil do Usuário

O usuário poderá possuir um perfil dentro da plataforma.

O perfil poderá apresentar:

- Nome de usuário;
- Foto;
- Publicações realizadas;
- Comentários;
- Conteúdos favoritos.

---

# 8. User Stories

## 8.1 Visitante

### US01 — Visualizar notícias

**Como** visitante,  
**quero** visualizar as principais notícias de Counter-Strike,  
**para** acompanhar os acontecimentos do cenário.

### US02 — Consultar partidas

**Como** visitante,  
**quero** consultar partidas futuras e resultados recentes,  
**para** acompanhar os campeonatos.

### US03 — Consultar jogadores

**Como** visitante,  
**quero** pesquisar jogadores profissionais,  
**para** consultar suas informações e estatísticas.

### US04 — Consultar equipes

**Como** visitante,  
**quero** visualizar informações sobre equipes profissionais,  
**para** acompanhar seus jogadores e resultados.

### US05 — Consultar campeonatos

**Como** visitante,  
**quero** visualizar campeonatos,  
**para** acompanhar sua programação e resultados.

### US06 — Pesquisar conteúdo

**Como** visitante,  
**quero** pesquisar jogadores, equipes e campeonatos,  
**para** encontrar rapidamente as informações desejadas.

---

## 8.2 Usuário

### US07 — Criar publicação

**Como** usuário autenticado,  
**quero** criar uma publicação na comunidade,  
**para** compartilhar opiniões e informações sobre Counter-Strike.

### US08 — Comentar

**Como** usuário autenticado,  
**quero** comentar em publicações,  
**para** participar das discussões da comunidade.

### US09 — Favoritar conteúdo

**Como** usuário autenticado,  
**quero** favoritar jogadores, equipes e notícias,  
**para** acessá-los posteriormente com facilidade.

### US10 — Gerenciar perfil

**Como** usuário autenticado,  
**quero** visualizar e editar meu perfil,  
**para** personalizar minha experiência na plataforma.

---

## 8.3 Administrador

### US11 — Moderar publicações

**Como** administrador,  
**quero** remover publicações inadequadas,  
**para** manter a comunidade organizada.

### US12 — Moderar comentários

**Como** administrador,  
**quero** remover comentários inadequados,  
**para** manter um ambiente saudável para os usuários.

### US13 — Gerenciar usuários

**Como** administrador,  
**quero** gerenciar usuários da plataforma,  
**para** controlar o acesso e a participação na comunidade.

---

# 9. Regras de Negócio

### RN01 — Cadastro

Cada usuário deverá possuir um identificador único dentro da plataforma.

### RN02 — Publicações

Somente usuários autenticados poderão criar publicações na área da comunidade.

### RN03 — Comentários

Somente usuários autenticados poderão realizar comentários.

### RN04 — Favoritos

Somente usuários autenticados poderão adicionar ou remover conteúdos dos favoritos.

### RN05 — Moderação

Administradores poderão remover publicações e comentários que violem as regras da comunidade.

### RN06 — Dados da API

As informações provenientes da API pública deverão ser apresentadas de acordo com os dados disponibilizados pelo serviço externo.

### RN07 — Indisponibilidade da API

Caso a API pública esteja indisponível, a aplicação deverá apresentar uma mensagem informando que os dados não puderam ser carregados.

### RN08 — Dados externos

O ClutchBR não deverá alterar os dados obtidos diretamente da API pública.

### RN09 — Inventários

Informações sobre inventários somente serão apresentadas quando estiverem disponíveis por meio de uma fonte compatível.

### RN10 — Responsabilidade sobre conteúdo

Os usuários serão responsáveis pelo conteúdo publicado na área da comunidade.

---

# 10. Requisitos Funcionais

### RF01

O sistema deverá apresentar uma página inicial com informações relevantes do cenário competitivo.

### RF02

O sistema deverá permitir a visualização de notícias.

### RF03

O sistema deverá permitir a visualização de partidas.

### RF04

O sistema deverá permitir a visualização de campeonatos.

### RF05

O sistema deverá permitir a consulta de equipes.

### RF06

O sistema deverá permitir a consulta de jogadores.

### RF07

O sistema deverá apresentar estatísticas disponibilizadas pela API.

### RF08

O sistema deverá permitir pesquisar jogadores e equipes.

### RF09

O sistema deverá permitir utilizar filtros.

### RF10

O sistema deverá permitir que usuários autenticados criem publicações.

### RF11

O sistema deverá permitir que usuários autenticados realizem comentários.

### RF12

O sistema deverá permitir que usuários autenticados favoritem conteúdos.

### RF13

O sistema deverá possuir área de perfil do usuário.

### RF14

O sistema deverá consumir dados da CS API.

### RF15

O sistema deverá utilizar uma API Fake para dados próprios da aplicação.

### RF16

O sistema deverá tratar erros relacionados à obtenção de dados da API.

### RF17

O sistema deverá possuir interface responsiva.

---

# 11. Requisitos Não Funcionais

### RNF01 — Responsividade

A aplicação deverá funcionar adequadamente em dispositivos desktop e mobile.

### RNF02 — Usabilidade

A interface deverá apresentar navegação simples e intuitiva.

### RNF03 — Desempenho

A aplicação deverá evitar carregamentos desnecessários de dados e recursos.

### RNF04 — Compatibilidade

A aplicação deverá funcionar nos principais navegadores modernos.

### RNF05 — Identidade Visual

A aplicação deverá utilizar um Design System consistente, incluindo cores, tipografia, espaçamentos e componentes.

### RNF06 — Arquitetura

O projeto deverá possuir organização modular dos arquivos e componentes.

### RNF07 — Framework CSS

A aplicação deverá utilizar o **Bootstrap 5** para construção de componentes e layouts responsivos.

### RNF08 — Código

O código deverá seguir padrões de organização e boas práticas de desenvolvimento.

### RNF09 — API

As requisições para APIs deverão possuir tratamento de erros.

### RNF10 — Acessibilidade

A aplicação deverá utilizar elementos semânticos e práticas básicas de acessibilidade.

---

# 12. Tecnologias Previstas

| Tecnologia | Utilização |
|---|---|
| HTML5 | Estrutura das páginas |
| CSS3 | Estilização complementar |
| Sass (SCSS) | Organização e gerenciamento dos estilos |
| Bootstrap 5 | Framework CSS e componentes |
| JavaScript | Interatividade e manipulação do DOM |
| JSON Server | Simulação da API própria |
| CS API | Dados do cenário competitivo de Counter-Strike |
| Git/GitHub | Versionamento do projeto |
| GitHub Pages | Hospedagem da aplicação |

---

# 13. Design e Identidade Visual

O ClutchBR utilizará uma identidade visual inspirada no universo competitivo de Counter-Strike e em plataformas modernas de esports.

A interface deverá priorizar:

- Tema escuro;
- Alto contraste;
- Elementos visuais relacionados a esports;
- Cards para organização das informações;
- Hierarquia visual clara;
- Layout responsivo;
- Navegação simples.

Os detalhes de cores, tipografia, espaçamentos e componentes serão definidos no documento **Design System**.

---

# 14. Escopo do MVP

A primeira versão funcional do ClutchBR deverá priorizar:

1. Página inicial;
2. Notícias;
3. Partidas;
4. Campeonatos;
5. Equipes;
6. Jogadores;
7. Estatísticas;
8. Pesquisa;
9. Integração com a CS API;
10. Área básica da comunidade;
11. Publicações;
12. Comentários;
13. Layout responsivo.

Funcionalidades como inventários de jogadores, sistema avançado de favoritos e outras integrações poderão ser implementadas posteriormente, de acordo com a viabilidade técnica e o tempo disponível.

---

# 15. Critérios de Sucesso

O projeto será considerado bem-sucedido quando:

- O usuário conseguir navegar pelas principais áreas da plataforma;
- Os dados da CS API forem apresentados corretamente;
- As páginas de jogadores e equipes forem funcionais;
- O usuário conseguir consultar partidas e campeonatos;
- A área da comunidade permitir interação entre usuários;
- A interface funcionar adequadamente em desktop e mobile;
- O Bootstrap 5 for utilizado na implementação dos componentes previstos;
- O projeto possuir Design System consistente;
- A aplicação estiver publicada no GitHub Pages;
- A documentação técnica estiver atualizada.

---

# 16. Evoluções Futuras

Após a implementação da primeira versão, poderão ser adicionadas novas funcionalidades, como:

- Integração com dados de inventário de jogadores profissionais;
- Histórico detalhado de skins;
- Valor estimado de inventários;
- Sistema de notificações;
- Sistema de seguidores;
- Perfil competitivo do usuário;
- Integração com Steam;
- Estatísticas mais avançadas;
- Sistema de ranking da comunidade;
- Cobertura de campeonatos em tempo real;
- Sistema de favoritos mais completo;
- Personalização da página inicial.
