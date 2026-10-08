# craft-tools

Versioni Linux x86_64 già compilate di due strumenti open source dell'ArtCraft team, per usarli da Claude in cloud senza ricompilarli.

| File | Programma | Sorgente |
|---|---|---|
| bin/pdfcraft-cli.gz | PdfCraft (tipo Acrobat Pro) | https://github.com/storytold/pdfcraft @ 7965b49 |
| bin/photocraft-cli.gz | PhotoCraft (tipo Photoshop) | https://github.com/storytold/photocraft @ c9a7d26 |

Installazione:

```sh
git clone --depth 1 https://github.com/millennio/craft-tools ~/craft-tools
mkdir -p ~/bin && for t in pdfcraft photocraft; do gunzip -c ~/craft-tools/bin/$t-cli.gz > ~/bin/$t-cli; chmod +x ~/bin/$t-cli; done
```

Licenza dei programmi: MIT OR Apache-2.0 (vedi i file LICENSE-*). Il nome e i loghi ArtCraft sono marchi dell'ArtCraft Team.
