# schema.data.gouv.fr

## Ajouter un schema

1. Fork repo
2. Add directory under `/schemas` with schema slug as name
3. Add a `source.yml` with the following content
4. Make a PR
5. Our build script will populate the `/schemas/<slug>` directory content with your schema

```yml
irve:
    source: https://github.com/etalab/schema-irve
    type:
        - TableSchema
        - Json
    author: Etalab
    licence: lov2
```

Expected repository layout:

```
|
|-- schema.<json|xsd|>
|-- README.md
```

|Type|Expected schema file|
|----|---------------|
|TableSchema|schema.json|
|XSD|schema.xsd|
|Json|schema.json|
