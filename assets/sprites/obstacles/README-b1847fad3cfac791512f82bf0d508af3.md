# assets/sprites/obstacles/

Sprites dos obstáculos para o mini-jogo **Fuga Romântica na Praça** (RunnerGame).

## Convenção de Nomenclatura

```
{categoria}_{descrição}_{índice:02d}.{extensão}
```

Todos os nomes em `snake_case`, letras minúsculas, sem espaços ou caracteres especiais.

## Dimensões

| Categoria | Tamanho do arquivo | Escala de exibição |
|-----------|--------------------|--------------------|
| Sprite de obstáculo | 32 × 32 px | 2× → 64 × 64 px |

## Arquivos Esperados

| Arquivo | Dimensões | Descrição | Status |
|---------|-----------|-----------|--------|
| `obstacle_bench_01.png` | 32 × 32 px | Banco de praça | [x] feito |
| `obstacle_hydrant_01.png` | 32 × 32 px | Hidrante | [ ] pendente |
| `obstacle_puddle_01.png` | 32 × 32 px | Poça d'água | [x] feito |
| `obstacle_dog_01.png` | 32 × 32 px | Cachorro | [ ] pendente |

## Arquivos Presentes

| Arquivo | Dimensões | Descrição | Status |
|---------|-----------|-----------|--------|
| `obstacle_bench_01.png` | 32 × 32 px | Banco de praça | [x] feito |
| `obstacle_bird_01.png` | 32 × 32 px | Pássaro (obstáculo aéreo) | [x] feito |
| `obstacle_puddle_01.png` | 32 × 32 px | Poça d'água | [x] feito |
| `obstacle_trash_01.png` | 32 × 32 px | Lixeira | [x] feito |

> **Nota:** Os arquivos `obstacle_bird_01.png` e `obstacle_trash_01.png` estão presentes mas não constavam na lista original do spec. Os arquivos `obstacle_hydrant_01.png` e `obstacle_dog_01.png` ainda estão pendentes.

## Notas

- O `PlayerAvatar` deve desviar dos obstáculos pulando ou agachando.
- Todos os sprites são exibidos em escala 2× (64 × 64 px na tela).
- Obstáculos são posicionados no chão da praça e se movem da direita para a esquerda com o scroll.
