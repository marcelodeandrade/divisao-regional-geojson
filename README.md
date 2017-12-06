# Divisão Regional

## Dados geoespaciais das regiões brasileiras, codificadas em [GeoJSON](http://geojson.org/).

# Estrutura

### O projeto está organizado da seguinte forma:

    .
    ├── examples                        # Contém exemplos de uso utilizando OpenLayers
    ├── src                             #
    │   ├── estados                     # GeoJson com informações dos Estados e seus municípios
    │   ├── regioes_imediatas           # GeoJson com informações das regiões imediatas
    │   └── regioes_intermediarias      # GeoJson com informações das regiões intermediárias
        
### Os `GeoJson` são do tipo `FeatureCollection` e possuem a seguinte estrutura conforme sua [especificação](https://geojson.org/geojson-spec.html):

    {
        "type": "FeatureCollection",
        "properties": {
            "codigo": 27,
            "uf": "AL",
            "nome": "Alagoas"
        },
        "features": [
            {
                "type": "Feature",
                "properties": {
                    "codigo": 2700102,
                    "nome": "Água Branca"
                },
                "geometry": {
                    "type": "Polygon",
                    "coordinates": [
                        [
                            [
                                -37.771,
                                -9.293
                            ],
                            ...
                        ]
                    ]
                }
            },
            ...
        ]
    }