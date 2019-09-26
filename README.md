# Taller sobre Folium

Para reproducir los contenidos de este taller en su computadora:

1. Descargue la plataforma [Anaconda](https://www.anaconda.com/) para su sistema operativo.
2. Clone los contenidos de este repositorio mediante [git](https://git-scm.com/) o descárguelos como un [archivo ZIP](https://github.com/mfvargas/taller-folium/archive/master.zip).
3. Abra los _notebooks_ (*.ipynb) con la versión de [Jupyter Notebook](https://jupyter.org/) que se instala junto con Anaconda.

Para descargar capas mediante WFS:
```bash
ogr2ogr -t_srs EPSG:4326 -f "GeoJSON" areas_conservacion.geojson WFS:"http://geos1pne.sirefor.go.cr/wfs?" "PNE:areas_conservacion"
ogr2ogr -t_srs EPSG:4326 -f "GeoJSON" transporte_ferroviario.geojson WFS:"http://geos.snitcr.go.cr/be/IGN_25/wfs?" "IGN_25:transporteferroviario_25k"
```
