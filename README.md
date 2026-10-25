# craft-tools

Versioni Linux x86_64 già compilate delle tredici **Crafting Apps** open source dell'ArtCraft team, per usarle da Claude in cloud senza ricompilarle (installazione in pochi secondi invece di circa un'ora).

| File | Programma | Alternativa a | Sorgente |
|---|---|---|---|
| bin/pdfcraft-cli.gz | PdfCraft | Acrobat Pro | https://github.com/storytold/pdfcraft @ c28d1c8 |
| bin/photocraft-cli.gz | PhotoCraft | Photoshop | https://github.com/storytold/photocraft @ b4a297f |
| bin/designcraft-cli.gz | DesignCraft | InDesign | https://github.com/storytold/designcraft @ 0f1ff65 |
| bin/vectorcraft-cli.gz | VectorCraft | Illustrator | https://github.com/storytold/vectorcraft @ 8bf090b |
| bin/effectcraft-cli.gz | EffectCraft | After Effects | https://github.com/storytold/effectcraft @ 9919048 |
| bin/filmcraft-cli.gz | FilmCraft | Premiere Pro | https://github.com/storytold/filmcraft @ bfc2384 |
| bin/lightcraft-cli.gz | LightCraft | Lightroom | https://github.com/storytold/lightcraft @ 38f8d25 |
| bin/wordcraft-cli.gz | WordCraft | Word | https://github.com/storytold/wordcraft @ b4da59f |
| bin/gridcraft-cli.gz | GridCraft | Excel | https://github.com/storytold/gridcraft @ 3099df9 |
| bin/deckcraft-cli.gz | DeckCraft | PowerPoint | https://github.com/storytold/deckcraft @ 6a1c735 |
| bin/figcraft-cli.gz | FigCraft | Figma | https://github.com/storytold/figcraft @ 9f78875 |
| bin/soundcraft-cli.gz | SoundCraft | Pro Tools | https://github.com/storytold/soundcraft @ ee050db |
| bin/cadcraft-cli.gz | CADCraft | AutoCAD | https://github.com/storytold/cadcraft @ b901656 |

## Installazione

```sh
git clone -q --depth 1 https://github.com/millennio/craft-tools ~/craft-tools
mkdir -p ~/bin && for f in ~/craft-tools/bin/*-cli.gz; do n=$(basename $f .gz); gunzip -c $f > ~/bin/$n; chmod +x ~/bin/$n; done
```

Strumenti per uso personale con Claude.

## Licenze

I programmi sono distribuiti con licenza MIT OR Apache-2.0 (vedi i file `LICENSE-*`). Il nome, il marchio e i loghi ArtCraft sono marchi dell'ArtCraft Team e non sono coperti da queste licenze.
