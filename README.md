# craft-tools

Versioni Linux x86_64 già compilate delle tredici **Crafting Apps** open source dell'ArtCraft team, per usarle da Claude in cloud senza ricompilarle (installazione in pochi secondi invece di circa un'ora).

| File | Programma | Alternativa a | Sorgente |
|---|---|---|---|
| bin/pdfcraft-cli.gz | PdfCraft | Acrobat Pro | https://github.com/storytold/pdfcraft @ eea00a6 |
| bin/photocraft-cli.gz | PhotoCraft | Photoshop | https://github.com/storytold/photocraft @ 1f984bf |
| bin/designcraft-cli.gz | DesignCraft | InDesign | https://github.com/storytold/designcraft @ 98d8016 |
| bin/vectorcraft-cli.gz | VectorCraft | Illustrator | https://github.com/storytold/vectorcraft @ 58e9851 |
| bin/effectcraft-cli.gz | EffectCraft | After Effects | https://github.com/storytold/effectcraft @ 79f6957 |
| bin/filmcraft-cli.gz | FilmCraft | Premiere Pro | https://github.com/storytold/filmcraft @ 5ed4952 |
| bin/lightcraft-cli.gz | LightCraft | Lightroom | https://github.com/storytold/lightcraft @ c50b74d |
| bin/wordcraft-cli.gz | WordCraft | Word | https://github.com/storytold/wordcraft @ a88e005 |
| bin/gridcraft-cli.gz | GridCraft | Excel | https://github.com/storytold/gridcraft @ 15c9d8c |
| bin/deckcraft-cli.gz | DeckCraft | PowerPoint | https://github.com/storytold/deckcraft @ e690829 |
| bin/figcraft-cli.gz | FigCraft | Figma | https://github.com/storytold/figcraft @ 53259cf |
| bin/soundcraft-cli.gz | SoundCraft | Pro Tools | https://github.com/storytold/soundcraft @ 7169dc4 |
| bin/cadcraft-cli.gz | CADCraft | AutoCAD | https://github.com/storytold/cadcraft @ d7ef7da |

## Installazione

```sh
git clone -q --depth 1 https://github.com/millennio/craft-tools ~/craft-tools
mkdir -p ~/bin && for f in ~/craft-tools/bin/*-cli.gz; do n=$(basename $f .gz); gunzip -c $f > ~/bin/$n; chmod +x ~/bin/$n; done
```

Strumenti per uso personale con Claude.

## Licenze

I programmi sono distribuiti con licenza MIT OR Apache-2.0 (vedi i file `LICENSE-*`). Il nome, il marchio e i loghi ArtCraft sono marchi dell'ArtCraft Team e non sono coperti da queste licenze.
