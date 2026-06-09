# ComicQuestRPG

A single-file RPG prototype for Comic Quest.

## Quick Art Swap Guide

The current root page uses one main comic image in `index.html`:

```text
assets/littlewing-lab.webp
```

To swap the picture, replace that file with a new image using the same name. That is the safest option because no code changes are needed.

## Recommended Image Size

Use this size for root-page comic art:

```text
1600 x 900 pixels
16:9 widescreen
.webp preferred
```

Good export settings:

```text
Format: WebP
Quality: 80-90
Max file size target: under 500 KB when possible
Color: RGB
```

A PNG or JPG can work too, but WebP keeps the site faster.

## Safe File Rules

Use lowercase file names with hyphens:

```text
littlewing-lab.webp
comicquest-intro.webp
labzero-door.webp
```

Avoid spaces in file names. Spaces work sometimes, but they make links easier to break.

## Slideshow-Friendly Folder Idea

When the page is ready for a slideshow setup, keep art in a dedicated folder:

```text
assets/slides/
```

Suggested slide names:

```text
assets/slides/slide-01.webp
assets/slides/slide-02.webp
assets/slides/slide-03.webp
```

Each slide should stay at:

```text
1600 x 900 pixels
```

That way the page can rotate images without resizing or jumping around.

## Current Image Code

In `index.html`, the current image path is set here:

```js
artImage.src = "assets/littlewing-lab.webp?v=20260608";
```

If you upload a new image with the same filename, update the version number at the end so browsers reload it:

```js
artImage.src = "assets/littlewing-lab.webp?v=20260609";
```

## Future Root Design Plan

A cleaner root design could use:

- a simple landing screen for Comic Quest
- one large slideshow frame for development art
- short buttons for Play Demo, Map, and Updates
- `assets/slides/` for easy picture swaps
- a small `slides` list in JavaScript so new images can be added without changing the layout
