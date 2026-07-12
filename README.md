# mapforge-icons

Public icon assets for MapForge/MapCraft, served via [jsDelivr](https://www.jsdelivr.com/)
so they resolve as plain, unauthenticated image URLs — usable both inside the editor and
in exported KML (Google Earth / Google My Maps fetch icon URLs directly, with no way to
authenticate against a protected host).

## Layout

One folder per icon category, so new categories can be added later without disturbing
existing ones:

- `pins/` — full pin-shaped marker replacements, numbered `pin-1.png` … `pin-N.png`.
  Each has its own pointed tip baked in (anchor at the bottom, not the center).

## URL format

```
https://cdn.jsdelivr.net/gh/idolevitt/mapforge-icons@main/<category>/<file>
```

e.g. `https://cdn.jsdelivr.net/gh/idolevitt/mapforge-icons@main/pins/pin-1.png`

jsDelivr caches `@main` for up to ~24h; if you replace a file and need it to update
immediately, use their [purge endpoint](https://www.jsdelivr.com/tools/purge) or reference
a version tag instead of `@main`.
