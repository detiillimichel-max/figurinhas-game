# figurinhas-game
# Ache a Figurinha Diferente

Jogo de achar a figurinha diferente — 3 figurinhas na tela (1 em cima, 2 embaixo), duas iguais e uma diferente.

## Como jogar
- Toque na figurinha que é diferente das outras duas.
- Você tem de 20 a 10 segundos por fase. O tempo diminui conforme avança.
- Vidas: 3 corações ❤️. Cada erro perde 1 coração.
- Se errar, a mesma fase repete mas com 2 segundos a menos.
- 3 erros = Game Over.

## Lógica das 20 fases
- **Fases 1-3:** diferença óbvia (emoji totalmente diferente)
- **Fases 4-6:** ligeiramente diferente (mudança de cor/hue)
- **Fases 7-9:** quase iguais (rotação leve)
- **Fases 10-13:** muito pouca diferença (tamanho 86%)
- **Fases 14-20:** grau máximo de dificuldade (brilho e matiz quase imperceptíveis)

Ao completar as 20 fases, o jogo volta para a fase 1 trocando todas as figurinhas (embaralha o baralho) e continua acumulando pontos.

## Pontuação
- Cada acerto vale `fase × 10` pontos.
- Ex: fase 1 = 10pts, fase 10 = 100pts, fase 20 = 200pts.

## Tempo
- Fase 1 começa com ~20s, fase 20 com ~10s.
- Fórmula: `tempo = round(20 - (fase-1)*10/19) - penalidade`
- Penalidade: +2s a menos a cada erro na mesma fase.

## Vidas
- Mostradas como corações no topo. Servem para "comprar" nova tentativa com menos tempo.

## Tecnologias
- Apenas `index.html` único, HTML + CSS + JS puro, responsivo detiillimichel-max.github.io/figurinhas-game/
- 
© 2026 Michel Detilli.
Todos os direitos reservados. 
É permitido jogar online. É proibida a cópia, distribuição ou uso comercial do código sem autorização.
