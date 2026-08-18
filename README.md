# Il tuo blog Jekyll

## Come pubblicarlo su GitHub Pages

1. Crea un repository su GitHub chiamato **tuonome.github.io** (sostituisci "tuonome" col tuo username GitHub — es. se il tuo username è `mrossi`, il repo si chiama `mrossi.github.io`).
2. Carica tutti questi file nel repository (root del repo, non in sottocartelle).
3. Apri `_config.yml` e modifica `title`, `description`, `author` e `url` con i tuoi dati.
4. Vai su **Settings → Pages** nel repository e verifica che la pubblicazione sia attiva dal branch `main`.
5. Aspetta 1-2 minuti: il sito sarà online su `https://tuonome.github.io`.

## Come scrivere un nuovo post

Crea un file dentro `_posts/` con questo nome: `AAAA-MM-GG-titolo-post.md`, es. `2026-09-01-il-mio-secondo-post.md`.

Contenuto del file:

```
---
layout: post
title: "Titolo del post"
date: 2026-09-01
---

Scrivi qui il contenuto in Markdown.
```

Fai commit e push: GitHub ricostruisce il sito automaticamente.

## Provarlo in locale (opzionale)

Se hai Ruby installato:

```
gem install bundler jekyll
bundle init
echo 'gem "jekyll"' >> Gemfile
bundle install
bundle exec jekyll serve
```

Poi apri `http://localhost:4000` nel browser.
