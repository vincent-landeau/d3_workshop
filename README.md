# Atelier D3.js

## Liens utiles - librairies

  - API D3.js : https://github.com/d3/d3/blob/master/API.md (v5)
  - API D3.js : https://github.com/d3/d3-3.x-api-reference/blob/master/API-Reference.md (v3)
  - En lien avec D3.js : https://github.com/wbkd/awesome-d3
  - Exemples de réalisations : http://christopheviau.com/d3list/gallery.html


## Liens utiles - données

  - Base Open data de données géo : https://geo.data.gouv.fr
  - Base de fichiers GeoJSON nationaux : https://github.com/gregoiredavid/france-geojson
  - Open data US : http://catalog.data.gov/dataset
  - Open data FR : http://data.gouv.fr/
  - Open data CA : http://ouvert.canada.ca/fr
  - Open data UK : http://data.gov.uk/
  - Open data EU : http://data.europa.eu/euodp
  - Open data NYC : https://opendata.cityofnewyork.us/
  - Open data SF : https://datasf.org/
  - Open data Paris : http://opendata.paris.fr/
  - Open data SNCF : https://data.sncf.com/
  - Open data Météo France : https://donneespubliques.meteofrance.fr/
  - US population stats : http://www.census.gov/data.html or http://www.socrata.com/discover/
  - CIA factbook : https://www.cia.gov/library/publications/the-world-factbook/
  - European Space Agency : https://earth.esa.int/web/guest/data-access/how-to-access-esa-data

  - Autres sources d'inspiration : https://www.forbes.com/sites/bernardmarr/2016/02/12/big-data-35-brilliant-and-free-data-sources-for-2016/#71341386b54d

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