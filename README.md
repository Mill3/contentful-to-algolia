# Transmit data from Contentful to Algolia

The application syncs content between Contentful and Algolia.
You can configure the service to run with Drafts (Preview API) from Contentful
and put it in different indexes in Algolia. The previx of each index can be
configured.

## Install the module

    npm install --save contentful-to-algolia

## Documentation

The main method of Sync:
- `sync(Array <types>, String <indexName>, [Function <callback>])`
  Sync multiple content types from Contentful to Algolia

## Usage

    // Require module
    const ContentfulToAlgolia = require('contentful-to-algolia');

    // Generate new instance
    const Sync = new ContentfulToAlgolia(Object <config>);

    // Sync data
    Sync.sync(
      Array <types>,
      String <indexName>,
      [Function <callback>]
    );


## Example config

You can find a sample configuration in [config.sample.js](./config.sample.js).

## Todo

* Remove elements which are not used anymore
* Use Contentful's Syncronisation API
* Tests
