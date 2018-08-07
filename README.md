# mono_dict_synth

## Monolingual

Monolingual sentences extracted from Wikipedia for English, Japanese and Basque.

Basque language dataset is smaller.

Japanese tokenized file was created using `mecab`.

```sh
cat ja.8M | mecab -O wakati > ja.8M.tok
```

Some stats.

```sh
wc *
```
lines|words|characters|file
---|---|---|---
   8000000|  159768014|  981898865| en.8M
   1583441|   21566657|  178533275| eu.1583K
   8000000|   11523656| 1233522530| ja.8M
   8000005|  275851648| 1505706066| ja.8M.tok


The files were split using `split` to overcome Github's 100MB-per-file restriction.
