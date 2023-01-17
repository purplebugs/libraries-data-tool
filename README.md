# Library Data Tool 📚 ⚒️

Convert data from library and related databases to formats to easily ingest into Elasticsearch

## Purpose 💖

Personal learning project to experiment with various solutions

## Workflow 🛤️

- Works: Book, Music, Film
- Persons: Author

```mermaid
flowchart LR;
    DATA_SOURCE_Library1_Works-->PubSub;
    DATA_SOURCE_Library2_Works-->PubSub;
    DATA_SOURCE_Metadata_generator_for_works-->PubSub;
    PubSub-->library-data-tool:::highlightclass;
    library-data-tool-->Elasticsearch;
    Elasticsearch-->Elastic_index_Works;
    Elasticsearch-->Elastic_index_Persons;
    Elasticsearch-->Elastic_index_Libraries;
    classDef highlightclass fill:#f96
```

## Usage 🤖

Pre-condition 🪴

`npm install`

Run app 🚀

`node index.js`

## Status 🚜

- Library works file: JSON -> NDJSON

## Credits 👏

- Example works data from [Deichman](https://deichman.no/)

## License 📝

The work is under exclusive copyright by default.
