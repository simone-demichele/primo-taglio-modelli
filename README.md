# primo-taglio-modelli

Copie dei modelli usati dall'app **Primo Taglio** (montaggio automatico di Reel per Adobe Premiere Pro).
L'app li scarica da qui al primo avvio. I file sono identici agli originali (stessa impronta SHA-256);
`model.bin` è diviso in due pezzi perché GitHub accetta file fino a 2 GB: l'app li riunisce e controlla il file intero.

Questo archivio contiene solo i modelli, non il codice dell'app.

## Contenuto (release `v1`)

| File | Origine | Licenza |
|---|---|---|
| `config.json`, `preprocessor_config.json`, `tokenizer.json`, `vocabulary.json`, `model.bin.001` + `model.bin.002` (= `model.bin`, 3 087 284 237 byte, SHA-256 `69f74147e3334731bc3a76048724833325d2ec74642fb52620eda87352e3d4f1`) | [Systran/faster-whisper-large-v3](https://huggingface.co/Systran/faster-whisper-large-v3), conversione CTranslate2 di [OpenAI Whisper large-v3](https://github.com/openai/whisper) | MIT (vedi sotto) |
| `it_core_news_lg-3.8.0-py3-none-any.whl` | [explosion/spacy-models, it_core_news_lg 3.8.0](https://github.com/explosion/spacy-models/releases/tag/it_core_news_lg-3.8.0), di Explosion AI | [CC BY-NC-SA 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/): solo uso non commerciale, con attribuzione, stessa licenza. Ridistribuito senza modifiche. |

## Licenze

**Whisper** — Copyright (c) 2022 OpenAI. **faster-whisper / conversione** — Copyright (c) 2023 SYSTRAN.
Licenza MIT:

> Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
> documentation files (the "Software"), to deal in the Software without restriction, including without limitation
> the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
> permit persons to whom the Software is furnished to do so, subject to the following conditions:
>
> The above copyright notice and this permission notice shall be included in all copies or substantial portions of
> the Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
> THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
> TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
> SOFTWARE.

**it_core_news_lg 3.8.0** — Explosion AI e autori dei dati di addestramento indicati nel pacchetto
(`meta.json`). Licenza Creative Commons Attribuzione - Non commerciale - Condividi allo stesso modo 3.0
(https://creativecommons.org/licenses/by-nc-sa/3.0/).
