# GUA map

An embeddable Leaflet map of the [Global University Academy](https://www.globaluniversityacademy.org/): partner universities and the teaching locations where courses are delivered.

**Live:** https://devottaenzo.github.io/gua-map/map.html

## Embed

```html
<div style="position:relative;width:100%;aspect-ratio:16/10;min-height:440px">
  <iframe src="https://devottaenzo.github.io/gua-map/map.html"
          title="Map of Global University Academy partners and teaching locations"
          loading="lazy"
          style="position:absolute;inset:0;width:100%;height:100%;border:0"></iframe>
</div>
```

See `embed-example.html` for a full page.

### URL options

| Parameter | Effect |
|---|---|
| `?type=member` / `teaching` | Show only one category |
| `?cluster=0` | Turn off marker clustering |
| `?scroll=1` | Enable scroll-wheel zoom immediately (otherwise it turns on after a click) |

## Editing the data

The `MEMBERS` and `TEACHING` lists are at the top of the script in `map.html`. Each row is `[name, city, lat, lng, url, note]`.

Partner list from globaluniversityacademy.org/about-us (checked 19 Nov 2026). Pins mark main campuses / headquarters and are approximate.

## Basemap and licences

- **Background map:** [OpenFreeMap](https://openfreemap.org) "Positron" style, rendered with MapLibre GL. Free for any use including commercial, no API key or account, no request limits. The only condition is attribution, which the map shows bottom-right: *OpenFreeMap © OpenMapTiles Data from © OpenStreetMap contributors*. Keep it visible.
- **Map data:** © OpenStreetMap contributors, under the [ODbL](https://www.openstreetmap.org/copyright).
- **Libraries:** Leaflet (BSD-2), Leaflet.markercluster (MIT), MapLibre GL JS (BSD-3), maplibre-gl-leaflet (ISC).

OpenFreeMap runs on donations; if GUA relies on it, a small recurring donation helps keep it running.
