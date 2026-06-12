# assets/sprites/notes/

Sprites das notas musicais para o mini-jogo **Ritmo do Coração** (RhythmGame).

## Convenção de Nomenclatura

```
{categoria}_{descrição}_{índice:02d}.{extensão}
```

Todos os nomes em `snake_case`, letras minúsculas, sem espaços ou caracteres especiais.

## Dimensões

| Categoria | Tamanho do arquivo | Escala de exibição |
|-----------|--------------------|--------------------|
| Nota do RhythmGame | 32 × 32 px | 1× → 32 × 32 px |

## Arquivos Esperados

| Arquivo | Dimensões | Cor sugerida | Coluna | Tecla | Status |
|---------|-----------|--------------|--------|-------|--------|
| `note_heart_col0_01.png` | 32 × 32 px | Rosa / Vermelho | 0 | A | [x] feito |
| `note_heart_col1_01.png` | 32 × 32 px | Azul / Ciano | 1 | S | [x] feito |
| `note_heart_col2_01.png` | 32 × 32 px | Verde / Lima | 2 | K | [x] feito |
| `note_heart_col3_01.png` | 32 × 32 px | Amarelo / Laranja | 3 | L | [x] feito |

## Notas

- Cada nota tem formato de coração (❤️) e uma cor distinta por coluna.
- As notas descem verticalmente na coluna correspondente e devem ser acertadas na `HitZone` com tolerância de ±150ms.
- Velocidade de queda: 400 px/s para `TRACK_WATP` (We Are The People) e 270 px/s para `TRACK_OLLG` (One Less Lonely Girl).
- Os sprites são exibidos em escala 1× (32 × 32 px na tela, sem escalonamento).
