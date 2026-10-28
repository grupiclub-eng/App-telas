# Human 1.0 — Canvas de UX

Wireframe de alta fidelidade estrutural construído com React Native, Expo, TypeScript, Expo Router e `StyleSheet`, apoiado pela [stack oficial](docs/TECH_STACK.md) do projeto.

## Rodar

```bash
pnpm install
pnpm start
```

Abra no Expo Go, simulador iOS, emulador Android ou Expo Web. O projeto inicia em um canvas não navegável com o Design System e todas as telas lado a lado, agrupadas pelos fluxos de autenticação, configurações, perfil, estados universais, notificações, formulários, listagens, navegação pós-login e componentes de mídia.

## Estrutura

- `app/`: entrada do Expo Router.
- `src/design-system/`: tokens, tipografia e componentes reutilizáveis.
- `src/core/`: adaptadores de infraestrutura compartilhados, como feedback tátil.
- `docs/TECH_STACK.md`: bibliotecas oficiais, responsabilidades e regras de adoção.
- `src/features/auth/authFlows.ts`: definição declarativa dos fluxos e telas.
- `src/features/auth/AuthScreen.tsx`: composição reutilizável das telas.
- `src/features/auth/AuthCanvas.tsx`: área de trabalho completa.
- `src/features/settings/`: telas e conteúdo simulado de configurações.
- `src/features/profile/`: telas e conteúdo simulado do perfil do usuário.
- `src/features/states/`: estados universais de carregamento, vazio, erro, sucesso e avisos.
- `src/features/notifications/`: telas do sistema de notificações com inbox, detalhe, permissão e vazio.
- `src/features/forms/`: conjunto completo de campos, seleções, controles e uploads simulados.
- `src/features/listings/`: padrões universais de lista, cards, grid, tabela, favoritos, recentes, histórico, busca, filtros e ordenação.
- `src/features/navigation/`: estrutura pós-autenticação com Home, pesquisa, notificações, perfil, drawer, bottom navigation, tabs, headers e barra de busca.
- `src/features/media/`: componentes de mídia para avatar, banner, carrossel, galeria, vídeo, áudio, PDF, QR Code e scanner.

## Próxima fase

Após a aprovação do UX, as mesmas definições e componentes podem ser conectados a rotas do Expo Router, estado de formulário, biometria, APIs e persistência segura sem reconstruir as telas.
