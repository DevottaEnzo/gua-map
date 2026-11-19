# GUA map

An embeddable Leaflet map of the [Global University Academy](https://www.globaluniversityacademy.org/): member universities, contributing partners, and the refugee camps where teaching happens (Azraq, Za'atari, Kakuma, Cox's Bazar).

**Live:** https://devottaenzo.github.io/gua-map/map.html

## Embed

```html
<div style="position:relative;width:100%;aspect-ratio:16/10;min-height:360px">
  <iframe src="https://devottaenzo.github.io/gua-map/map.html"
          title="Map of Global University Academy partners and teaching locations"
          loading="lazy"
          style="position:absolute;inset:0;width:100%;height:100%;border:0;border-radius:8px"></iframe>
</div>
```

See `embed-example.html` for a full page.

### URL options

| Parameter | Effect |
|---|---|
| `?type=member` / `contributor` / `teaching` | Show only one category |
| `?cluster=0` | Turn off marker clustering |
| `?scroll=1` | Enable scroll-wheel zoom immediately (otherwise it turns on after a click) |

## Editing the data

The `MEMBERS`, `CONTRIBUTORS` and `TEACHING` lists are at the top of the script in `map.html`. Each row is `[name, city, lat, lng, url, note]`.

Partner list from globaluniversityacademy.org/about-us (checked 19 Nov 2026). Pins mark main campuses / headquarters and are approximate.

## Basemap

Tiles are Esri World Light Gray (no API key). Esri's terms ask commercial sites to use a free ArcGIS Location Platform account; alternatively swap the tile URL in `map.html` for MapTiler, Stadia or Mapbox.
