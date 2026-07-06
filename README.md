# 🎮 Dona Anna: A Caça aos Óculos

Um **campo minado** de fliperama com estética **grunge 2.5D** (vibe Street Fighter/Sega) e tom irônico. Dona Anna, 96 anos, só quer passear pelo jardim da fazenda que tanto ama — mas sem os óculos não enxerga nada, e o jardim está cheio de perigos (🐍 cobra, 🪜 escada escorregadia, 🧑‍⚕️ o fisioterapeuta que ela evita, 👵 a vizinha chata...). As "minas" são esses perigos; revele todas as casas seguras para achar os óculos e curtir o passeio. O número numa casa revelada indica quantos perigos há nas casas vizinhas. Feito em **um único arquivo HTML**, sem dependências, sem build.

## Como jogar
- Digite seu **nome** no pop-up inicial (obrigatório para o ranking)
- **Clique:** revelar uma casa
- **Marcar cilada:** arraste a **bandeirinha 🚩** (canto direito) até a casa suspeita — funciona no celular (clique direito também marca no desktop)
- A **primeira jogada é sempre segura** (você nunca morre de cara)
- Limpe todas as casas seguras → **👓 Dona Anna acha os óculos!**

## Pontuação e ranking
- Cada fase começa com uma base (**1500 / 2500 / 3500**) e perde 1 ponto por segundo
- **+50** por cada cilada descoberta · **−100** por cada cilada não descoberta (game over)
- Toda partida (vitória ou derrota) é salva no ranking, com **nome, data, fase e pontos**
- No fim aparecem os **TOP 3** e o resultado/posição da sua partida
- Controles de **🔊 Som On/Off**, **🎵 Música On/Off** e volume **+/−** no menu

## Acesso
O jogo é protegido por uma **senha da família** (portão na tela inicial). É um cadeado leve, client-side — mantém o jogo restrito a quem tem o convite. A senha não fica em texto no código (apenas o hash).

## Como rodar
Abra o arquivo direto no navegador:
```
open index.html
```
Ou sirva localmente (recomendado, garante que áudio/localStorage funcionem bem):
```
python3 -m http.server 8000
# depois abra http://localhost:8000
```

## Tecnologias
- HTML + CSS + JavaScript vanilla (1 arquivo, zero dependências)
- Visual 2.5D com CSS 3D transforms (`perspective` + `rotateX`) e ruído grunge via SVG `feTurbulence`
- Arte 100% emoji + CSS/SVG (sem assets externos)
- Áudio de fliperama sintetizado com a Web Audio API
- Melhor tempo salvo em `localStorage`

## Dificuldades
| Modo | Grade | Perigos |
|------|-------|---------|
| 🛋️ Sonequinha | 9×9 | 10 |
| 🧺 Dia de feira | 16×16 | 40 |
| 👨‍👩‍👧 Os netos vêm almoçar | 16×30 | 99 |

---
© Fazenda Grunge Games • Insert Coin • 1 Player
