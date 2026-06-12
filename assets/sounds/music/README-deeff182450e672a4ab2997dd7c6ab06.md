# assets/sounds/music/

Arquivos de música e beat maps para o mini-jogo **Ritmo do Coração** (RhythmGame).

## Convenção de Nomenclatura

```
{categoria}_{descrição}_{índice:02d}.{extensão}   ← para arquivos de áudio
{categoria}_{descrição}.{extensão}                 ← para arquivos de beat map (sem índice)
```

Todos os nomes em `snake_case`, letras minúsculas, sem espaços ou caracteres especiais.

## Arquivos Esperados

### Músicas

| Arquivo | Formato | BPM | Dificuldade | Velocidade das notas | Descrição | Status |
|---------|---------|-----|-------------|----------------------|-----------|--------|
| `music_watp_01.mp3` | MP3 | ~126 BPM | Alta | 400 px/s | "We Are The People" — Empire Of The Sun | [ ] pendente |
| `music_ollg_01.mp3` | MP3 | ~85 BPM | Normal | 270 px/s | "One Less Lonely Girl" — Justin Bieber | [ ] pendente |

### Beat Maps

| Arquivo | Formato | Faixa associada | Descrição | Status |
|---------|---------|-----------------|-----------|--------|
| `beatmap_watp.json` | JSON | `music_watp_01.mp3` | Beat map de "We Are The People" | [ ] pendente |
| `beatmap_ollg.json` | JSON | `music_ollg_01.mp3` | Beat map de "One Less Lonely Girl" | [ ] pendente |

## Formato do Beat Map

Cada arquivo `.json` deve conter uma lista de eventos no seguinte formato:

```json
[
  { "timestampMs": 1234, "columnIndex": 0 },
  { "timestampMs": 1734, "columnIndex": 2 },
  ...
]
```

- `timestampMs` — milissegundos exatos em que a nota deve ser gerada (relativo ao início da música).
- `columnIndex` — coluna onde a nota aparece: `0` (tecla A), `1` (tecla S), `2` (tecla K), `3` (tecla L).

## Identificadores Internos

| ID interno | Arquivo de música | Arquivo de beat map |
|------------|-------------------|---------------------|
| `TRACK_WATP` | `music_watp_01.mp3` | `beatmap_watp.json` |
| `TRACK_OLLG` | `music_ollg_01.mp3` | `beatmap_ollg.json` |

## Notas

- O `BeatSynchronizer` carrega o beat map correspondente à faixa selecionada pelo jogador.
- O tempo de referência para sincronização é `Music.getPosition()` (em segundos), convertido para ms.
- Desvios de até ±20ms são corrigidos a cada frame para compensar imprecisões do `deltaTime` acumulado.
- Densidade máxima de notas simultâneas: 3 para `TRACK_WATP`, 2 para `TRACK_OLLG`.
