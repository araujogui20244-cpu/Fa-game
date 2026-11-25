# Super Bomberman 5 PLUS

Projeto de expansão não oficial para Super Bomberman 5.

## Organização

- `game/upstream/`: base original ligada como submódulo Git, fixada no commit `fea95b2c824819ca68ff32a3e4079af6aa4a99a0`.
- `plus/`: código e documentação exclusivos do PLUS.
- `third_party/`: dependências externas isoladas.
- `.github/workflows/android.yml`: compilação Android automática.

O submódulo contém o código-fonte do projeto-base. O GitHub Actions usa `submodules: recursive` para obter também as dependências declaradas pela base.

## Objetivos do PLUS

- Preservar a campanha, os modos e as músicas originais.
- Acrescentar a opção MULTIPLAYER ao menu.
- NORMAL GAME cooperativo para dois jogadores.
- BATTLE para até quatro jogadores.
- Criar uma continuação da campanha com mundos, fases e chefes novos.
- Gerar APK Android.

## Estado real

A base original e o fluxo de compilação Android estão conectados. O workflow foi adicionado e é acionado por push na branch `main` ou manualmente na aba Actions.

**As funcionalidades exclusivas do PLUS ainda não foram implementadas.** O APK gerado pelo workflow neste estágio é a base original, não a expansão completa. A campanha extra e a nova tela MULTIPLAYER exigem alterações adicionais no código e testes.

Não inclua ROMs, saves ou conteúdo protegido no repositório. O app solicita a ROM do próprio usuário no primeiro uso. Consulte os avisos de licença da base e das dependências antes de redistribuir.

Base: https://github.com/MauricioSuporte/SuperBomberman5SNESRecomp
