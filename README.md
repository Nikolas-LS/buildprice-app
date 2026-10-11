# BuildPrice

[![Flutter](https://img.shields.io/badge/Flutter-3.13+-02569B?logo=flutter&logoColor=white)](https://flutter.dev) [![Dart](https://img.shields.io/badge/Dart-3.13+-0175C2?logo=dart&logoColor=white)](https://dart.dev)

**BuildPrice** é um aplicativo multiplataforma para **estimativa e gestão de custos de construção**, pensado para tornar orçamentos de obra mais rápidos, transparentes e acessíveis no canteiro, no escritório ou em visita ao cliente.

---

## Problema e proposta de valor

No mercado da construção civil, orçamentos costumam depender de planilhas dispersas, preços desatualizados e cálculos manuais repetitivos. O **BuildPrice** centraliza:

- **Estimativas** a partir de parâmetros da obra (tipologia, áreas, quantitativos e demais variáveis do escopo)
- **Referência de preços** de insumos e serviços para apoiar a composição do orçamento
- **Visão clara do custo total** e detalhamento para cliente ou equipe técnica

---

## Público-alvo

| Perfil | Uso principal |
|--------|----------------|
| Engenheiros e arquitetos | Orçamentos preliminares e revisões |
| Empreiteiros e construtoras | Propostas comerciais e controle de custo |
| Mestres de obra / equipe de campo | Consulta rápida de quantitativos e valores |
| Estudantes | Apoio a disciplinas de orçamento e obra |

---

## Funcionalidades

### Planejadas

- Cadastro de projetos e obras
- Formulários por tipologia ou etapa construtiva
- Cálculo automático de custos (materiais, mão de obra e encargos conforme regras do produto)
- Histórico e comparação de orçamentos
- Exportação e compartilhamento de relatórios
- Experiência otimizada para uso em campo (quando aplicável)

### Estado atual do repositório

Este repositório contém a **estrutura base Flutter** (multiplataforma). As telas e regras de negócio do BuildPrice serão implementadas nas próximas iterações.

---

## Stack técnica

| Camada | Tecnologia |
|--------|------------|
| App | [Flutter](https://flutter.dev) |
| Linguagem | [Dart](https://dart.dev) SDK `^3.13.5` |
| Plataformas | Android, iOS, Web, Windows, Linux, macOS |
| Dependências principais | `cupertino_icons`; `flutter_lints` (dev) |

---

## Pré-requisitos

- [Flutter SDK](https://docs.flutter.dev/get-started/install) compatível com o `pubspec.yaml` (Dart 3.13+)
- Android Studio e/ou Xcode, conforme a plataforma alvo
- Editor com suporte a Dart/Flutter (VS Code ou Android Studio)

Verifique o ambiente:

```bash
flutter doctor
```

---

## Como executar

Clone o repositório e instale as dependências:

```bash
git clone https://github.com/Nikolas-LS/buildprice-app.git
cd buildprice-app
flutter pub get
```

Execute no dispositivo ou emulador:

```bash
flutter run
```

Build de release (exemplo Android):

```bash
flutter build apk --release
```

Mais opções de publicação: [documentação de deployment do Flutter](https://docs.flutter.dev/deployment).

---

## Estrutura do projeto

```
lib/
├── main.dart          # Entrada do aplicativo
├── core/              # Temas, rotas, constantes (previsto)
├── features/          # Módulos por funcionalidade (previsto)
└── shared/            # Widgets e utilitários (previsto)
```

---

## Roadmap

| Fase | Entrega |
|------|---------|
| **Base** | Projeto Flutter multiplataforma e pipeline de build |
| **MVP** | Fluxo principal de orçamento (entrada de dados + resultado) |
| **v1.0** | Persistência local, histórico e exportação de relatório |
| **Futuro** | Integrações, conta de usuário e sincronização (se previsto) |
