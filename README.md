# Atelier D3.js

Notes :
  - Si Chrome se plaint de requêtes "cross-origin" locales, le lancer avec le flag "--allow-file-access-from-files"

  - Pour récupérer des fichiers géographiques directement en GeoJSON : https://github.com/gregoiredavid/france-geojson

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