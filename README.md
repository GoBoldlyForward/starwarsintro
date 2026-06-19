# starwarsintro.css

A pure CSS library for creating a Star Wars-style intro crawl. No JavaScript dependencies.

> **Note on naming:** the name references a third-party trademark. Kept as-is — this is a non-commercial homage plugin, low risk in practice.

## Demo

[goboldlyforward.github.io/starwarsintro](https://goboldlyforward.github.io/starwarsintro/)

## What it does

Drops a Star Wars-style scrolling intro crawl onto any page using pure CSS animations. Useful for fan sites, movie marathons, browser-game intros, presentations, or any project where the recognizable crawl effect fits.

## Install

```bash
npm install @goboldlyforward/starwarsintro
```

```css
@import "@goboldlyforward/starwarsintro/starwarsintro.css";
```

Or link it straight from a CDN — the star-field background (`img/stars-bg.jpg`) ships with the package and loads automatically:

```html
<link rel="stylesheet" href="https://unpkg.com/@goboldlyforward/starwarsintro/starwarsintro.css">
```

The stylesheet references `img/stars-bg.jpg` relatively, so if you self-host, keep that image next to the CSS (both are in this repo).

## Usage

Wrap your intro content in the structure below:

```html
<div class="star-wars-intro">

  <!-- Blue intro text -->
  <p class="intro-text">
    A few days ago, during...
  </p>

  <!-- Logo image or text -->
  <h2 class="main-logo">
    <img src="img/your-logo.png">
  </h2>

  <!-- Scrolling content -->
  <div class="main-content">
    <div class="title-content">
      <p class="content-header">Your Title</p>
      <p class="content-body">
        Your scrolling story goes here. As it scrolls, the text recedes into the distance and fades out, in the iconic opening-crawl style.
      </p>
    </div>
  </div>
</div>
```

## Roadmap

This plugin is undergoing modernization. Tracked work:

- [x] LICENSE (MIT)
- [x] `.gitignore`
- [x] README
- [x] `package.json`
- [x] Update CSS header (rebrand Polar Notion → Go Boldly Forward)
- [x] Remove legacy artifacts (`.DS_Store`, `starwarsintro.css.zip`)
- [x] Strip obsolete vendor prefixes (`-webkit/-moz/-ms/-o`) and fix broken gradient syntax
- [x] Update demo page (drop legacy jQuery + Bootstrap, drop JotForm, native smooth-scroll, rebrand)
- [x] Refresh demo with the shared Go Boldly Forward plugin design system (light + dark, Inter, `.gbf-*` markup, yellow accent)
- [x] Publish to npm (as `@goboldlyforward/starwarsintro`)
- [ ] Optional `starwarsintro-rails` gem wrapper
- [ ] GitHub Actions CI (stylelint)

## License

MIT — see [LICENSE](LICENSE).
