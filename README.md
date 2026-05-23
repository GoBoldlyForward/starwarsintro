# starwarsintro.css

A pure CSS library for creating a Star Wars-style intro crawl. No JavaScript dependencies.

> **Note on naming:** the current name uses a third-party trademark and will be renamed before npm publication. See [Roadmap](#roadmap).

## Demo

[goboldlyforward.github.io/starwarsintro](https://goboldlyforward.github.io/starwarsintro/)

## What it does

Drops a Star Wars-style scrolling intro crawl onto any page using pure CSS animations. Useful for fan sites, movie marathons, browser-game intros, presentations, or any project where the recognizable crawl effect fits.

## Install

For now, download `starwarsintro.css` from this repo. (npm publication is pending a rename — see Roadmap.)

```html
<link rel="stylesheet" href="path/to/starwarsintro.css">
```

You'll also need a star-field background image at `img/stars-bg.jpg` (included in this repo).

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
- [ ] Remove legacy artifacts (`.DS_Store`, `starwarsintro.css.zip`)
- [ ] Strip obsolete vendor prefixes (`-webkit/-moz/-ms/-o`)
- [ ] Update demo page (drop legacy jQuery + Bootstrap, remove Polar Notion branding)
- [ ] Rename — required before npm publish (Disney IP)
- [ ] Publish to npm
- [ ] Optional Rails gem wrapper
- [ ] GitHub Actions CI (stylelint)

## License

MIT — see [LICENSE](LICENSE).
