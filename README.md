<div align="center">

<img src="https://raw.githubusercontent.com/AndreFecury/AndreFecury/main/assets/jogo.svg" width="480" alt="Jogo de terror 3D em Unity" />

# Happy Tree Friends · Jogo de Terror 3D

Jogo de terror em primeira pessoa feito na **Unity** com **C#**.

![Unity](https://img.shields.io/badge/Unity_2019.3-000000?style=for-the-badge&logo=unity&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D4?style=for-the-badge&logo=windows&logoColor=white)

[![Baixar o jogo](https://img.shields.io/badge/Baixar_o_jogo-Windows_.zip-C0392B?style=for-the-badge&logo=github&logoColor=white)](../../releases/latest)

</div>

## História

Sete pessoas desapareceram perto de uma mansão abandonada, cercada por uma floresta escura. Você é um repórter que vai até lá investigar. Para provar o que aconteceu, precisa encontrar os objetos deixados pelos desaparecidos, enquanto um monstro ronda a floresta e pode te encontrar a qualquer momento.

Projeto final em grupo do curso de desenvolvimento de jogos do **CETAM**.

## Como jogar

1. Baixe o `.zip` na [página de releases](../../releases/latest).
2. Extraia **a pasta inteira** (o jogo precisa da pasta `Happy Tree Friends_Data` e do `UnityPlayer.dll` ao lado do executável).
3. Abra `Happy Tree Friends.exe`.

## Controles

| Tecla | Ação |
|---|---|
| W A S D | Andar |
| Mouse | Olhar ao redor |
| Shift | Correr (gasta stamina) |
| Ctrl | Agachar |
| 1 | Prancheta com a lista de itens a encontrar |
| 2 | Lanterna |
| 3 | Machado |
| F | Ligar e desligar a lanterna |
| Botão esquerdo | Usar o machado |
| Esc | Pausar |

## Mecânicas

- **Stamina:** correr cansa; a respiração e o som dos passos mudam conforme o ritmo.
- **Lanterna com bateria:** a carga acaba com o uso e pode ser recarregada com pilhas espalhadas pelo mapa.
- **Coleta de evidências:** cada item encontrado é marcado na prancheta.
- **Machado:** abre caminho para novas áreas.
- **Monstro com IA:** patrulha a floresta com NavMesh, tem campo de visão e persegue o jogador quando o vê. Se você for pego, vem o jumpscare.

## Estrutura do código

```
Assets/
├── Scripts/
│   ├── Movimento.cs           # andar, correr, agachar, stamina e sons de passos
│   ├── Lanterna.cs            # lanterna com consumo e recarga de bateria
│   ├── GerenteDeItens.cs      # troca entre prancheta, lanterna e machado
│   ├── GerenteUIPrancheta.cs  # lista de itens coletados
│   ├── ColecionarItem.cs      # coleta de itens e pilhas
│   ├── RandomPatrol.cs        # IA do monstro: patrulha, visão e perseguição
│   ├── JumpscareManager.cs    # jumpscare e tela de game over
│   ├── MenuDePause.cs         # menu de pausa
│   └── ...                    # cutscenes de entrada e saída, machado, câmera
└── Script/
    ├── MenuUI.cs              # menu principal
    └── ChamadaController.cs   # vídeo de abertura
```

## Abrindo o projeto

O projeto usa a **Unity 2019.3.15f1**. Este repositório contém o código e as configurações do projeto. Os modelos, sons e pacotes da Unity Asset Store não foram incluídos por questões de licença e de tamanho.

---

<div align="center"><sub>Feito por <a href="https://github.com/AndreFecury">André Fecury</a> · Manaus, AM</sub></div>
