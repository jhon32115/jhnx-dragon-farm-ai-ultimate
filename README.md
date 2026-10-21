# JHNX Dragon Farm AI Ultimate

Aplicativo Android para automação assistida de atividades repetitivas no Minecraft Bedrock, com foco em Dragon Ball, acessibilidade, macros, perfis, reconhecimento visual local e compilação em GitHub Actions.

## Introdução

Este repositório entrega uma base funcional e modular para construir a aplicação JHNX Dragon Farm AI Ultimate. A implementação foi iniciada com a primeira fase do plano de desenvolvimento: projeto compilável, armazenamento local, motor de automação, interface principal em Compose e testes de regra central de pausa e parada de emergência.

## Status atual

- Projeto Android inicial configurado.
- Câmara de estado para automação com pausa manual persistente, suspensão por perda de foco e parada de emergência.
- Interface principal com painel de status e ações de controle.
- Repositório preparado para build via GitHub Actions.

## Recursos implementados

- Configuração de projeto Android com Gradle.
- Interface principal em Jetpack Compose.
- Motor de automação com machine state.
- Pausa manual prioritária.
- Suspensão automática ao perder o foco.
- Parada total de emergência.
- Repositório de preferências locais.
- Testes unitários para regras de automação.
- Workflow de build em GitHub Actions.

## Recursos experimentais

- Captura visual e OCR ainda não habilitados em produção.
- Módulos específicos de Dragon Evolution, combate, chefes e transformações seguem como extensões configuráveis.
- Serviços de acessibilidade e sobreposição ainda precisam ser conectados ao fluxo real do jogo.

## Requisitos

- Android Studio Ladybug ou mais recente.
- JDK 17.
- Android SDK 34.
- Gradle (via wrapper quando disponível).

## Estrutura da pasta

- `app/` — módulo Android principal.
- `app/src/main/java/` — código da aplicação.
- `app/src/test/java/` — testes unitários.
- `.github/workflows/` — build automatizado.

## Como configurar o projeto

1. Clone o repositório.
2. Abra no Android Studio.
3. Aguarde o Gradle sincronizar.
4. Configure o SDK Android 34.
5. Instale o JDK 17.

## Como compilar

- No Android Studio: Run > Run 'app'.
- Via terminal: `./gradlew testDebugUnitTest assembleDebug`

## Como instalar o APK

1. Gere o APK de debug.
2. Transfira para o celular.
3. Instale o arquivo `.apk`.
4. Autorize as permissões solicitadas.

## Limitações conhecidas

- Não há integração real com o Minecraft Bedrock confirmada no ambiente atual.
- Não existem coordenadas de jogo ou macros reais validadas para Dragon Evolution.
- A captura de tela e reconhecimento visual são implementados como base extensível e não garantem precisão em todos os celulares.
- A geração do wrapper do Gradle não foi executada neste ambiente, portanto a compilação precisa ser validada no ambiente local ou no GitHub Actions.

## Checklist de testes

- [ ] Instalar o APK.
- [ ] Autorizar acessibilidade.
- [ ] Testar coordenada simples.
- [ ] Iniciar sequência curta.
- [ ] Pausar manualmente.
- [ ] Verificar que não houve retomada indevida.
- [ ] Retomar manualmente.
- [ ] Sair do jogo e verificar suspensão.
- [ ] Rodar parada de emergência.
- [ ] Validar logs.

## Próximo passo recomendado

Implementar a segunda fase do plano: serviço de acessibilidade, gesto de toque e calibração de coordenadas, seguido de macros e perfis reais.
