# 🎮 Warriors of Freedom

**Warriors of Freedom** é um jogo 3D de ação tática em terceira pessoa desenvolvido com **Unreal Engine**.

O jogador assume o controle de um soldado de elite enviado para uma operação de alto risco: **infiltrar-se em uma base inimiga, enfrentar forças hostis, localizar reféns mantidos em cativeiro e conduzi-los em segurança até o ponto de extração**.

Além de sua proposta como jogo, o projeto possui finalidade acadêmica e educacional. O mesmo conjunto de mecânicas será desenvolvido em duas abordagens distintas dentro da Unreal Engine:

- 🔷 **Blueprints**
- 💻 **C++**

Essa estrutura permite comparar o desenvolvimento visual baseado em Blueprints com a implementação tradicional por meio de programação orientada a objetos em C++.

---

## 📖 Sobre o projeto

O **Warriors of Freedom** foi concebido como um projeto de estudo e desenvolvimento de jogos 3D utilizando a Unreal Engine.

O projeto explora diferentes áreas envolvidas na construção de um jogo de ação em terceira pessoa, incluindo:

- movimentação de personagens;
- sistema de câmera em terceira pessoa;
- sistema de combate;
- armas e munições;
- sistema de vida e dano;
- animações;
- inteligência artificial;
- patrulhamento de inimigos;
- percepção do jogador;
- perseguição e combate;
- sistema de objetivos;
- interação com elementos do cenário;
- resgate de reféns;
- interface gráfica;
- efeitos sonoros;
- efeitos visuais;
- level design;
- organização arquitetural de projetos Unreal Engine.

O objetivo é desenvolver progressivamente um jogo funcional e, simultaneamente, construir um material de referência para estudos sobre desenvolvimento de jogos utilizando **Blueprints e C++**.

---

# 🎯 Premissa

Uma instalação militar foi tomada por forças inimigas.

Um grupo de reféns encontra-se preso dentro da base e uma operação de resgate precisa ser executada.

O jogador controla um soldado de elite responsável por realizar a missão.

A operação envolve quatro objetivos principais:

1. infiltrar-se na base inimiga;
2. neutralizar ou evitar as forças hostis;
3. localizar e libertar os reféns;
4. conduzir os sobreviventes até o ponto de extração.

A missão será considerada concluída quando os objetivos estabelecidos forem cumpridos e os reféns forem resgatados com sucesso.

---

# 🕹️ Gênero

O projeto combina elementos de:

- **Third-Person Shooter — TPS**
- ação;
- combate tático;
- infiltração;
- inteligência artificial;
- exploração;
- resgate.

---

# 🔁 Gameplay Loop

O ciclo principal de gameplay segue inicialmente a seguinte estrutura:

```text
Explorar
   ↓
Observar o ambiente
   ↓
Identificar ameaças
   ↓
Evitar ou enfrentar inimigos
   ↓
Avançar pela base
   ↓
Localizar os reféns
   ↓
Libertar os reféns
   ↓
Chegar ao ponto de extração
   ↓
Concluir a missão
```

---

# 🧩 Duas implementações

Uma das principais características acadêmicas do projeto é possuir duas versões da mesma aplicação.

## 🔷 Blueprint Edition

Versão desenvolvida utilizando principalmente o sistema de programação visual da Unreal Engine.

```text
game/
└── blueprint/
```

Nesta versão serão utilizados recursos como:

- Blueprint Classes;
- Blueprint Interfaces;
- Actor Components;
- Event Graphs;
- Animation Blueprints;
- Behavior Trees;
- Blackboards;
- Widgets;
- Data Assets;
- sistemas de eventos.

---

## 💻 C++ Edition

Versão desenvolvida utilizando C++ integrado à Unreal Engine.

```text
game/
└── cpp/
```

Esta implementação explora conceitos como:

- programação orientada a objetos;
- classes;
- herança;
- composição;
- encapsulamento;
- Actor Components;
- Unreal Property System;
- delegates;
- interfaces;
- comunicação entre C++ e Blueprints;
- arquitetura de sistemas de gameplay.

O objetivo não é eliminar o uso de Blueprints na versão C++, mas demonstrar como sistemas centrais podem ser implementados em código e posteriormente expostos para utilização dentro da Unreal Engine.

---

# 🧠 Comparação Blueprint × C++

Durante o desenvolvimento, diferentes sistemas serão implementados nas duas abordagens.

| Sistema | Blueprints | C++ |
|---|:---:|:---:|
| Movimentação do jogador | ✅ | ✅ |
| Sistema de vida | ✅ | ✅ |
| Sistema de dano | ✅ | ✅ |
| Sistema de armas | ✅ | ✅ |
| Disparo | ✅ | ✅ |
| Munição | ✅ | ✅ |
| Recarga | ✅ | ✅ |
| Interação | ✅ | ✅ |
| Inteligência artificial | ✅ | ✅ |
| Sistema de objetivos | ✅ | ✅ |
| Resgate de reféns | ✅ | ✅ |
| HUD | ✅ | ✅ |

Essa abordagem permite analisar as vantagens, limitações e características de cada forma de desenvolvimento.

---

# 🪖 Player

O jogador controla um soldado de elite especializado em operações de infiltração e resgate.

Entre as mecânicas previstas estão:

- movimentação;
- corrida;
- agachamento;
- controle de câmera;
- mira;
- disparo;
- recarga;
- troca de armas;
- interação com objetos;
- sistema de vida;
- recebimento de dano;
- morte.

Outras mecânicas poderão ser incorporadas conforme a evolução do projeto.

---

# 🔫 Sistema de combate

O sistema de combate será desenvolvido progressivamente.

Entre os principais recursos previstos estão:

- armas de fogo;
- sistema de disparo;
- munição;
- carregadores;
- recarga;
- dano;
- pontos de vida;
- efeitos de impacto;
- efeitos sonoros;
- efeitos visuais;
- mira;
- diferentes tipos de armas.

Inicialmente, o projeto utilizará um conjunto reduzido de armas para manter o escopo controlado.

---

# 🤖 Inteligência Artificial

Os inimigos utilizarão sistemas de inteligência artificial fornecidos pela Unreal Engine.

Entre os recursos estudados estão:

- AI Controller;
- Behavior Tree;
- Blackboard;
- AI Perception;
- Navigation System;
- NavMesh;
- Tasks;
- Services;
- percepção visual;
- percepção sonora;
- patrulhamento;
- investigação;
- perseguição;
- combate.

Um inimigo poderá assumir diferentes estados de comportamento.

```text
Patrol
   ↓
Suspicious
   ↓
Alert
   ↓
Combat
   ↓
Search
   ↓
Patrol
```

O objetivo é criar inimigos capazes de reagir dinamicamente às ações do jogador.

---

# 🎯 Sistema de missão

A primeira missão será estruturada em torno da invasão da base inimiga.

Exemplo de sequência:

```text
Insertion
   ↓
Infiltration
   ↓
Enemy Base
   ↓
Locate Hostages
   ↓
Rescue Hostages
   ↓
Extraction
   ↓
Mission Complete
```

Os objetivos poderão ser exibidos dinamicamente no HUD.

Exemplo:

```text
MISSION OBJECTIVES

☑ Enter the enemy base
☑ Locate the hostages
☐ Rescue the hostages
☐ Reach the extraction point
```

---

# 🆘 Sistema de reféns

Os reféns constituem um dos principais elementos da missão.

Inicialmente, cada refém poderá possuir estados como:

```text
Captured
   ↓
Released
   ↓
Following
   ↓
Extracted
```

O jogador deverá localizar os personagens, interagir com eles e conduzi-los até uma área segura.

O sistema poderá posteriormente ser expandido com novos comportamentos e estados.

---

# 🗺️ Level Design

O projeto utilizará mapas separados para desenvolvimento, testes e missões.

Exemplo:

```text
Maps/
├── Prototype/
├── Training/
└── Missions/
```

## Prototype

Mapa utilizado para testes isolados de mecânicas.

Exemplos:

- movimentação;
- armas;
- animações;
- inteligência artificial;
- interação;
- HUD.

## Training

Área destinada à experimentação das principais mecânicas do jogador.

## Missions

Contém os mapas utilizados nas missões oficiais do jogo.

A primeira fase será uma **base militar inimiga**.

---

# 📂 Estrutura do repositório

A estrutura principal do projeto está organizada da seguinte maneira:

```text
warriors-of-freedom/
│
├── README.md
├── LICENSE
├── .gitignore
├── .gitattributes
│
├── game/
│   │
│   ├── blueprint/
│   │   ├── Config/
│   │   └── Content/
│   │
│   └── cpp/
│       ├── Config/
│       ├── Content/
│       └── Source/
│
├── docs/
│   ├── game-design/
│   ├── architecture/
│   ├── gameplay/
│   ├── artificial-intelligence/
│   ├── level-design/
│   ├── assets/
│   ├── development/
│   ├── academic/
│   └── images/
│
├── assets/
│   ├── licenses/
│   └── references/
│
├── shared/
│
├── prototypes/
│
├── tests/
│
├── scripts/
│
└── releases/
```

---

# 🏗️ Arquitetura

A arquitetura do projeto procura separar os diferentes sistemas responsáveis pelo gameplay.

Entre os principais módulos encontram-se:

```text
Warriors of Freedom
│
├── Characters
│   ├── Player
│   ├── Enemies
│   └── Hostages
│
├── AI
│
├── Weapons
│
├── Components
│
├── Interaction
│
├── Mission
│
├── Rescue
│
├── UI
│
├── Audio
│
└── Game
```

Na implementação C++, será dada preferência à utilização de componentes reutilizáveis.

Exemplo:

```text
Player Character
│
├── Health Component
├── Weapon Component
├── Interaction Component
└── Inventory Component
```

Essa abordagem reduz o acoplamento entre sistemas e facilita a reutilização das funcionalidades.

---

# 🛠️ Tecnologias

O projeto utiliza ou poderá utilizar as seguintes tecnologias e ferramentas:

### Game Engine

- Unreal Engine

### Programação

- Blueprints
- C++

### Desenvolvimento

- Visual Studio
- Git
- GitHub
- Git LFS

### Modelos e animações

- Mixamo
- Fab
- Unreal Engine Marketplace / Epic Games

Outras ferramentas poderão ser incorporadas conforme as necessidades do desenvolvimento.

---

# 🎨 Assets externos

O projeto poderá utilizar assets provenientes de plataformas externas.

Entre elas:

- Adobe Mixamo;
- Fab;
- Epic Games;
- Unreal Engine Marketplace;
- outras bibliotecas de assets compatíveis com Unreal Engine.

Os respectivos direitos autorais e licenças permanecem pertencentes aos seus autores e fornecedores.

Sempre que possível, os assets externos utilizados serão documentados em:

```text
assets/external-assets.md
```

Pacotes comerciais ou conteúdos cuja licença não permita redistribuição **não serão disponibilizados diretamente neste repositório**.

A documentação do projeto poderá indicar a origem e os procedimentos necessários para obtenção desses recursos.

---

# 📦 Git LFS

Projetos Unreal Engine possuem diversos arquivos binários de grande tamanho.

Por esse motivo, o projeto utiliza **Git Large File Storage — Git LFS** para determinados tipos de arquivos, incluindo:

```text
.uasset
.umap
.fbx
.wav
.tga
```

Dependendo do tamanho e das condições de licença, determinados assets externos poderão não ser versionados no GitHub.

---

# 🚀 Como executar

## Pré-requisitos

Antes de executar o projeto, certifique-se de possuir:

- Unreal Engine instalada;
- Git;
- Git LFS;
- Visual Studio com suporte para desenvolvimento C++, caso utilize a versão C++.

Clone o repositório:

```bash
git clone https://github.com/SEU-USUARIO/warriors-of-freedom.git
```

Acesse o diretório:

```bash
cd warriors-of-freedom
```

Para utilizar Git LFS:

```bash
git lfs install
```

```bash
git lfs pull
```

Depois escolha a implementação desejada.

### Blueprint

```text
game/blueprint/
```

Abra o arquivo `.uproject` correspondente utilizando a Unreal Engine.

### C++

```text
game/cpp/
```

Abra o arquivo `.uproject`.

Quando necessário, gere novamente os arquivos de projeto do Visual Studio e compile a aplicação.

> Dependendo dos assets externos utilizados, poderá ser necessário realizar configurações adicionais descritas na documentação do projeto.

---

# 🗺️ Roadmap

O desenvolvimento inicial está dividido nas seguintes etapas.

### Fase 1 — Core Gameplay

- [ ] Criar projeto base
- [ ] Configurar personagem
- [ ] Implementar movimentação
- [ ] Implementar câmera TPS
- [ ] Configurar sistema de Input

### Fase 2 — Combat

- [ ] Criar sistema de armas
- [ ] Implementar disparo
- [ ] Implementar munição
- [ ] Implementar recarga
- [ ] Criar sistema de vida
- [ ] Implementar sistema de dano
- [ ] Implementar morte

### Fase 3 — Artificial Intelligence

- [ ] Criar inimigo básico
- [ ] Configurar NavMesh
- [ ] Implementar patrulhamento
- [ ] Implementar percepção
- [ ] Implementar perseguição
- [ ] Implementar combate
- [ ] Implementar busca pelo jogador

### Fase 4 — Mission System

- [ ] Criar sistema de objetivos
- [ ] Criar Mission Manager
- [ ] Criar triggers
- [ ] Implementar atualização de objetivos
- [ ] Implementar conclusão de missão

### Fase 5 — Hostage Rescue

- [ ] Criar personagem refém
- [ ] Implementar interação
- [ ] Implementar libertação
- [ ] Implementar acompanhamento do jogador
- [ ] Implementar ponto de extração

### Fase 6 — Interface

- [ ] Criar HUD
- [ ] Indicador de vida
- [ ] Indicador de munição
- [ ] Indicador de objetivos
- [ ] Menu principal
- [ ] Tela de conclusão da missão

### Fase 7 — Polish

- [ ] Implementar efeitos visuais
- [ ] Implementar efeitos sonoros
- [ ] Melhorar animações
- [ ] Melhorar iluminação
- [ ] Refinar Level Design
- [ ] Balancear gameplay

### Fase 8 — Blueprint × C++

- [ ] Consolidar versão Blueprint
- [ ] Consolidar versão C++
- [ ] Documentar diferenças de implementação
- [ ] Criar exemplos comparativos
- [ ] Documentar boas práticas

---

# 🎓 Finalidade acadêmica

O **Warriors of Freedom** também funciona como um ativo acadêmico destinado ao estudo de:

- desenvolvimento de jogos digitais;
- Unreal Engine;
- programação visual;
- programação C++;
- orientação a objetos;
- arquitetura de software aplicada a games;
- inteligência artificial para jogos;
- desenvolvimento de sistemas de gameplay;
- animação;
- level design;
- interfaces;
- gerenciamento de projetos de jogos;
- versionamento utilizando Git e GitHub.

O projeto pode ser utilizado como referência em aulas, exercícios, demonstrações técnicas e experimentações acadêmicas.

Um dos principais objetivos educacionais é demonstrar como uma mesma mecânica pode ser implementada utilizando diferentes abordagens.

```text
Gameplay System
        │
        ├── Blueprint Implementation
        │
        └── C++ Implementation
```

Dessa maneira, é possível compreender não apenas **como construir uma determinada funcionalidade**, mas também analisar diferentes soluções arquiteturais para o mesmo problema.

---

# 📚 Documentação

Documentações adicionais estão disponíveis no diretório:

```text
docs/
```

Entre os assuntos documentados estarão:

- Game Design Document;
- arquitetura;
- gameplay;
- inteligência artificial;
- sistemas de armas;
- personagens;
- missões;
- sistema de resgate;
- Level Design;
- assets;
- instalação;
- desenvolvimento;
- comparação entre Blueprints e C++.

---

# 🔖 Versionamento

O projeto utiliza Git para controle de versão.

As versões estáveis poderão ser disponibilizadas através da área **Releases** do GitHub.

Exemplo de evolução planejada:

```text
v0.1.0 — Player Movement
v0.2.0 — Combat Prototype
v0.3.0 — Enemy AI
v0.4.0 — Mission System
v0.5.0 — Hostage Rescue
v0.6.0 — Complete Mission
v0.9.0 — Beta
v1.0.0 — First Complete Version
```

---

# 🤝 Contribuições

O projeto possui finalidade acadêmica e está em desenvolvimento contínuo.

Sugestões, estudos, experimentações e melhorias poderão ser incorporados conforme a evolução do ativo.

---

# ⚖️ Licença

A licença referente ao código-fonte e aos materiais produzidos especificamente para o **Warriors of Freedom** será definida no arquivo:

```text
LICENSE
```

Assets, personagens, animações, modelos, texturas, sons e demais recursos provenientes de terceiros permanecem sujeitos às licenças estabelecidas pelos respectivos autores e distribuidores.

---

# 👨‍💻 Autor

Projeto desenvolvido por **André Olímpio**.

Professor de Tecnologia da Informação e desenvolvedor de projetos acadêmicos voltados às áreas de:

- Desenvolvimento de Software
- Programação
- Banco de Dados
- Inteligência Artificial
- Desenvolvimento Web
- Desenvolvimento Mobile
- Desenvolvimento de Jogos Digitais
- Engenharia de Software

---

## 🎮 Warriors of Freedom

> **Infiltrate. Fight. Rescue. Extract.**

Projeto acadêmico desenvolvido com **Unreal Engine, Blueprints e C++**.
