# ComicQuestRPG

A single-file RPG prototype for Comic Quest.

## Current Build

The playable demo starts at:

```text
index.html
```

The extra pocket-check page is:

```text
one-cig.html
```

## Current Art

The root page uses this image:

```text
assets/littlewing-lab.png
```

Current export:

```text
700 x 564 pixels
PNG
```

To swap the picture, replace that file with a new image using the same name. That is the safest option because no code changes are needed.

## Recommended Production Art

When the comic panel art is final, keep a high-quality source file outside the repo and export a game-ready copy into `assets/`.

Suggested target:

```text
1600 x 900 pixels
WebP preferred for final web builds
PNG is fine when browser/local preview reliability matters
```

Use lowercase file names with hyphens:

```text
littlewing-lab.png
comicquest-intro.webp
labzero-door.webp
```

Avoid spaces in file names. Spaces work sometimes, but they make links easier to break.

## Cleanup Notes

The old `characters.html`, `inventory.html`, `quests.html`, and `map.html` redirect pages were removed. The current demo only keeps pages that are part of the active prototype.