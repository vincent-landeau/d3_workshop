# Atelier D3.js

## Liens utiles

  - API D3.js : https://github.com/d3/d3/blob/master/API.md (v5)
  - API D3.js : https://github.com/d3/d3-3.x-api-reference/blob/master/API-Reference.md (v3)
  - Base Open data de données géo : https://geo.data.gouv.fr
  - Base de fichiers GeoJSON nationaux : https://github.com/gregoiredavid/france-geojson
  - Convertir un fichier .shp en geojson : http://www.weblog.eliaz.fr/article120.html
  - Fonctionnement général D3.js : https://bl.ocks.org/mbostock/3808218


Notes :
  - Préférer Firefox pour vos tests (cf cahier des charges)
  - Si vous testez sur Chrome, le lancer avec le flag "--allow-file-access-from-files" pour charger des fichiers locaux
  - Charger des données pour un pie chart sur C3.js

```javascript
d3.json('data/pie_c3.json', function(data) {
    var chart = c3.generate({
        bindto: '#chart',
        data: {
            json: data,
            type: 'pie'
        }
    })
});
```