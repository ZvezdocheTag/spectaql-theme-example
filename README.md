# SpectaQL theme usage example

This is an example Node.js project using the [SpectaQL dark theme](https://github.com/anvilco/spectaql-dark-theme) with [SpectaQL](https://github.com/anvilco/spectaql) to generate GraphQL documentation. It is minimal in an effort to show you how to integrate SpectaQL and a custom theme into your own app.

The result looks like this:

<img width="1792" alt="screenshot-desktop" src="https://user-images.githubusercontent.com/69169/171294193-cc50d146-75e8-4749-928b-cc3b6a81d2b7.png">

## Usage

Usage is simple: install the dependencies, then build your docs. It uses SpectaQL's example schema.

```sh
yarn install

# Run the docs on a dev server
yarn docs:develop

# Build the static site HTML
yarn docs:build
```

You can fork the example and point it to your own schema by updating the [introspection](https://github.com/anvilco/spectaql/blob/857ac01fc02070854b5f7abfad3b41ce2ec44602/config-example.yml#L42) key in [`spectaql-config.yml`](/spectaql-config.yml).

## Local theme

Instead of using a theme from NPM, you can use a local directory as a theme. Fork this project, create a local theme directory, and update the [`spectaql.themeDir`](https://github.com/anvilco/spectaql/blob/857ac01fc02070854b5f7abfad3b41ce2ec44602/config-example.yml#L33) yaml key to point to your local theme directory.

See the [theme readme](https://github.com/anvilco/spectaql/tree/main/examples/themes) for more details.