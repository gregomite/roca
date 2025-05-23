<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [@hulu/roca](#huluroca)
  - [Documentation](#documentation)
  - [Contributing](#contributing)
    - [Modifying the docs site](#modifying-the-docs-site)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# @hulu/roca

BrightScript unit testing.  No device required.

## Documentation

All of our documentation is at [hulu.github.io/roca](https://hulu.github.io/roca). If you'd prefer to view the raw markdown that powers the doc site, it's all in the [docs/](docs/) folder.

## Contributing

If you spot a bug or want a feature, please feel free to file an issue. If you want to contribute code yourself, simply fork the repo and open a PR.

### Releasing / Publishing a New NPM Package

1. Ensure that you've got a clean working state by pulling a fresh copy of `main`.
2. Bump the package version (following semver best practices) via `yarn version` and merge back into `main`.
3. Run the prepublishing tests and packaging steps: `yarn run prepublishOnly`.
4. Assuming all tests passed and the package was correctly built, you can now publish via `yarn publish`.

_**Note:** You'll need a privileged account to publish package updates. See **"NPM Package Management Access"** below for more information._

### NPM Package Management Access

The package registry for this project is located at npmjs.com: [@hulu/roca](https://www.npmjs.com/package/@hulu/roca). Only privileged members are able to publish new updates. If you need to be granted privileges, reach out to one of the repository owners and [have them add you](https://www.npmjs.com/settings/hulu/members).

### Modifying the docs site

We use [docsify](https://docsify.js.org) to build our site, and [Github pages](https://pages.github.com/) to deploy it. To run the documentation site locally, simply run:
```shell
$ yarn serve-docs
```

Any changes you make to files in the `docs/` directory will cause the server to automatically reload the page.
