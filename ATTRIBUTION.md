# Quellen und Namensnennung der Daten in diesem Repository

Datensätze der Spiegelwelt „Pavillon Ratscher“ (https://github.com/mynametouse/pavillon-ratscher). Erzeugt und veröffentlicht von
GitHub Actions; diese Datei schreibt die Aktion `suhl-publish` bei jeder Veröffentlichung neu. Lizenz und Namensnennung reisen mit
den Daten: jedes Produkt nennt sie in seiner `index.json` (der Boden in `meta.json`).

## Suhl (`suhl/`)

### Bäume – `suhl/b/v2/` (Stand 2026-11-13, Gebiet stadt)

Luftbild (DOP20 RGB und CIR, Bildflug 15.05.2024): © GDI-Th, CC BY 4.0 (dl-de/by-2-0); Bäume, Baumreihen, Wald- und Grünflächen: © OpenStreetMap-Mitwirkende, ODbL 1.0; Objekthöhen nDOM1 (Laser 2020–2025): © GDI-Th, CC BY 4.0, bezogen über easygeodata.de
- Digitale Orthophotos Thüringen 20 cm (WMS th_dop, th_dop20cir) – CC BY 4.0 – https://www.geoproxy.geoportal-th.de/geoproxy/services/DOP
- OpenStreetMap – ODbL 1.0 – https://www.openstreetmap.org/copyright
- ETHOS.BUILDA – Gebäudebestand Deutschland (Grundriss, Höhe), Thüringen aus dem LoD2 des Landes – ODbL 1.0 – https://zenodo.org/records/11845992
- Normalisiertes Oberflächenmodell nDOM1 (Objekthöhen 1 m, DOM1 − DGM1) Thüringen – CC BY 4.0 – https://easygeodata.de

### Gelände und Luftbild – `suhl/boden/v2/` (Stand 2026-11-13, Gebiet stadt)

Luftbild: © GDI-Th (CC BY 4.0) · Gelände: Copernicus DEM GLO-30, © DLR e.V. 2010-2014 und © Airbus Defence and Space GmbH 2014-2018, bereitgestellt im Rahmen von COPERNICUS durch EU und ESA · Geländemodell DGM1: © GDI-Th (CC BY 4.0), bezogen über easygeodata.de · Landbedeckung (Kronenabzug im Gelände): © ESA WorldCover project 2021 (CC BY 4.0) · Gebietsgrenzen und Straßenkorridore: © OpenStreetMap-Mitwirkende (ODbL)
- terrain: DGM1 Thüringen (1 m, © GDI-Th, CC BY 4.0), außerhalb Copernicus DEM GLO-30 mit abgesenktem Wald
- terrain_source: dgm1+cop30
- imagery: DOP Thüringen, WMS TH DOP (th_dop, 20 cm), © GDI-Th, CC BY 4.0
- imagery_flight: 2024-05-15 über der ganzen Gemeinde (th_dop_info, tools/suhl/out/bestand/luftbild.json); Veröffentlichung 2025-02; Bezug bDOM
- areas: Gebiete und Ortsteile: tools/suhl/out/bestand/gebiete.geojson; Korridore: tools/suhl/boden/korridor.json (© OpenStreetMap-Mitwirkende, ODbL 1.0)

### Szenario-Zahlen – `suhl/d/v2/` (Stand 2026-11-13, Gebiet stadt)

Gebäude: ETHOS.BUILDA, Forschungszentrum Jülich (ODbL 1.0), aus LoD2 Thüringen © GDI-Th · Gebäudefunktion, Geschosse, Adressen: ALKIS © GDI-Th (CC BY 4.0) · © OpenStreetMap-Mitwirkende (ODbL) · Luftbild: © GDI-Th (CC BY 4.0) · Oberflächenmodell: DOM1 © GDI-Th (CC BY 4.0) – bezogen über easygeodata.de · Angaben zu Bauten und Vierteln: eigene Recherche · Gelände: DGM1 © GDI-Th (CC BY 4.0) · © Statistische Ämter des Bundes und der Länder (Zensus 2022, Gitterdaten; Datenlizenz Deutschland – Namensnennung – Version 2.0; Abruf 2026-11-13)
- ETHOS.BUILDA – Gebäudebestand Deutschland (Grundriss, Höhe), Thüringen aus dem LoD2 des Landes – ODbL 1.0 – https://zenodo.org/records/11845992
- ALKIS vereinfacht – Gebäude und Bauwerke (WFS adv_alkis_wfs, ave:GebaeudeBauwerk) – CC BY 4.0 – https://www.geoproxy.geoportal-th.de/geoproxy/services/adv_alkis_wfs
- OpenStreetMap – ODbL 1.0 – https://www.openstreetmap.org/copyright
- Digitale Orthophotos Thüringen 20 cm (WMS th_dop, th_dop20cir) – CC BY 4.0 – https://www.geoproxy.geoportal-th.de/geoproxy/services/DOP
- Digitales Oberflächenmodell DOM1 Thüringen (1 m) – CC BY 4.0 – bezogen über easygeodata.de – https://geoportal.thueringen.de/gdi-th/download-offene-geodaten
- Recherche des Projekts (docs/plans/suhl/*.md, Quellen dort je Angabe) – eigene Zusammenstellung – https://github.com/mynametouse/pavillon-ratscher/tree/src/docs/plans/suhl
- Regeln und Annahmen der Pipeline (als Schätzung gekennzeichnet) – –
- Digitales Geländemodell DGM1 Thüringen (1 m) – CC BY 4.0 – https://geoportal.thueringen.de/gdi-th/download-offene-geodaten
- Zensus 2022, Gitterdaten 100 m (Stichtag 15.05.2022; Werte zur Geheimhaltung leicht verändert) – dl-de/by-2-0 – https://www.zensus2022.de

### Gebäude – `suhl/g/v2/` (Stand 2026-11-13, Gebiet stadt)

Gebäude: ETHOS.BUILDA, Forschungszentrum Jülich (ODbL 1.0), aus LoD2 Thüringen © GDI-Th · Gebäudefunktion, Geschosse, Adressen: ALKIS © GDI-Th (CC BY 4.0) · © OpenStreetMap-Mitwirkende (ODbL) · Luftbild: © GDI-Th (CC BY 4.0) · © Statistische Ämter des Bundes und der Länder, Zensus 2022 · Oberflächenmodell: DOM1 © GDI-Th (CC BY 4.0) – bezogen über easygeodata.de · Angaben zu Bauten und Vierteln: eigene Recherche · Gelände: DGM1 © GDI-Th (CC BY 4.0)
- ETHOS.BUILDA – Gebäudebestand Deutschland (Grundriss, Höhe), Thüringen aus dem LoD2 des Landes – ODbL 1.0 – https://zenodo.org/records/11845992
- ALKIS vereinfacht – Gebäude und Bauwerke (WFS adv_alkis_wfs, ave:GebaeudeBauwerk) – CC BY 4.0 – https://www.geoproxy.geoportal-th.de/geoproxy/services/adv_alkis_wfs
- OpenStreetMap – ODbL 1.0 – https://www.openstreetmap.org/copyright
- Digitale Orthophotos Thüringen 20 cm (WMS th_dop, th_dop20cir) – CC BY 4.0 – https://www.geoproxy.geoportal-th.de/geoproxy/services/DOP
- Zensus 2022, Gitterdaten 100 m: Gebäude nach Baujahr – offene Daten mit Quellenangabe (Lizenzname für die Gitterdaten nicht geprüft) – https://www.zensus2022.de
- Digitales Oberflächenmodell DOM1 Thüringen (1 m) – CC BY 4.0 – bezogen über easygeodata.de – https://geoportal.thueringen.de/gdi-th/download-offene-geodaten
- Recherche des Projekts (docs/plans/suhl/*.md, Quellen dort je Angabe) – eigene Zusammenstellung – https://github.com/mynametouse/pavillon-ratscher/tree/src/docs/plans/suhl
- Regeln und Annahmen der Pipeline (als Schätzung gekennzeichnet) – –
- Digitales Geländemodell DGM1 Thüringen (1 m) – CC BY 4.0 – https://geoportal.thueringen.de/gdi-th/download-offene-geodaten

### Grünflächen – `suhl/gr/v2/` (Stand 2026-11-13, Gebiet stadt)

© OpenStreetMap-Mitwirkende, ODbL 1.0
- OpenStreetMap – ODbL 1.0 – https://www.openstreetmap.org/copyright
- Digitale Orthophotos Thüringen 20 cm (WMS th_dop, th_dop20cir) – CC BY 4.0 – https://www.geoproxy.geoportal-th.de/geoproxy/services/DOP

### Möbel der Straße – `suhl/m/v2/` (Stand 2026-11-13, Gebiet stadt)

© OpenStreetMap-Mitwirkende (ODbL 1.0); Haltestellennamen des Fahrplans: DELFI e.V. über gtfs.de (CC BY 4.0)
- OpenStreetMap – ODbL 1.0 – https://www.openstreetmap.org/copyright
- Soll-Fahrplandaten Deutschland (GTFS, gtfs.de aus DELFI) – CC BY 4.0 – https://gtfs.de/de/feeds/
- Regeln und Annahmen der Pipeline (als Schätzung gekennzeichnet) – –

### Straßenraum – `suhl/s/v2/` (Stand 2026-11-13, Gebiet stadt)

Straßen, Wege, Plätze © OpenStreetMap-Mitwirkende (ODbL 1.0); Höhen: Copernicus DEM GLO-30 (© DLR e.V. 2010-2014 und © Airbus Defence and Space GmbH 2014-2018, bereitgestellt unter COPERNICUS durch die Europäische Union und ESA), Geländekacheln von suhl-boden, wo vorhanden (© GDI-Th, CC BY 4.0)
- OpenStreetMap – ODbL 1.0 – https://www.openstreetmap.org/copyright
- Digitales Geländemodell DGM1 Thüringen (1 m) – CC BY 4.0 – https://geoportal.thueringen.de/gdi-th/download-offene-geodaten
- Copernicus DEM GLO-30 (Oberflächenmodell 30 m) – Copernicus DEM licence – https://copernicus-dem-30m.s3.amazonaws.com/
- ESA WorldCover 2021 v200 (Landbedeckung 10 m) – CC BY 4.0 – https://esa-worldcover.org

### Waldbestände (Zellen 20 m) – `suhl/w/v2/` (Stand 2026-11-13, Gebiet stadt)

Luftbild (DOP20 RGB und CIR, Bildflug 15.05.2024): © GDI-Th, CC BY 4.0 (dl-de/by-2-0); Bäume, Baumreihen, Wald- und Grünflächen: © OpenStreetMap-Mitwirkende, ODbL 1.0; Objekthöhen nDOM1 (Laser 2020–2025): © GDI-Th, CC BY 4.0, bezogen über easygeodata.de
- Digitale Orthophotos Thüringen 20 cm (WMS th_dop, th_dop20cir) – CC BY 4.0 – https://www.geoproxy.geoportal-th.de/geoproxy/services/DOP
- OpenStreetMap – ODbL 1.0 – https://www.openstreetmap.org/copyright
- Normalisiertes Oberflächenmodell nDOM1 (Objekthöhen 1 m, DOM1 − DGM1) Thüringen – CC BY 4.0 – https://easygeodata.de
