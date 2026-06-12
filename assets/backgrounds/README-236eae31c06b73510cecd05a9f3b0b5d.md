# assets/backgrounds/

Imagens de fundo (backgrounds) para todos os mini-jogos do projeto.

## Convenção de Nomenclatura

```
{categoria}_{descrição}_{índice:02d}.{extensão}
```

Todos os nomes em `snake_case`, letras minúsculas, sem espaços ou caracteres especiais.

## Dimensões

| Categoria | Tamanho do arquivo | Escala de exibição |
|-----------|--------------------|--------------------|
| Background (tela cheia) | 480 × 270 px | 4× → 1920 × 1080 px |

## Arquivos Esperados

| Arquivo | Dimensões | Mini-jogo | Descrição | Status |
|---------|-----------|-----------|-----------|--------|
| `background_rhythm_01.png` | 480 × 270 px | RhythmGame | Palco com luzes de neon nas cores favoritas | [x] feito |
| `background_plaza_01.png` | 480 × 270 px | RunnerGame | Praça com scroll horizontal (paralaxe) | [x] feito |
| `background_treasure_reveal_01.png` | 480 × 270 px | TreasureGame | Imagem escondida revelada ao remover blockers | [x] feito |
| `background_cutscene_final_01.png` | 480 × 270 px | RunnerGame | Imagem estática da cutscene final ("A salvo! ❤️") | [x] feito |
| `background_dressup_01.png` | 480 × 270 px | DressUpGame | Fundo para a tela de montagem de personagem | [ ] pendente |

## Notas

- Todos os backgrounds são pixel art em resolução 480 × 270 px.
- São exibidos em escala 4× na tela (1920 × 1080 px em fullscreen).
- O `background_treasure_reveal_01.png` é a imagem que fica escondida sob os `BlockerObject` no TreasureGame — deve ser uma foto/sprite do namorado fazendo coração com as mãos.
- O `background_cutscene_final_01.png` deve mostrar os dois personagens no banco da praça com cesta de piquenique.
