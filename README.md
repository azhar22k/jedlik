# jedlik

Jedlik is an extensible DynamoDB ODM for Node

Jedlik allows you to create plain JavaScript classes to represent entities in your domain.
Extending these classes from Jedlik's `Model` class enhances the class by introducing behaviour to allow it to interact with DynamoDB in a simple way.

## Install

Yarn:
`yarn add @peak-ai/jedlik`
NPM:
`npm i -S @peak-ai/jedlik`

Unstable releases are published as `develop` - e.g. `yarn add @peak-ai/jedlik@develop`

## Usage

## API
#### static `query(key, [index = null])`

## Development
### Getting Started
- `git clone git@github.com:PeakBI/jedlik.git`
- `yarn`

### Build
- `yarn build` uses babel and rollup to output two builds:
- - a CommonJS build in `dist`
- - a ES Module build in `es`

### Test
- `yarn test` will run unit tests using Jest

### Publish
- Use `yarn publish` to publish the package to the npm registry.
- When developing, if you need to test a change on another project you have two options:
- - **Preferred** - in the `package.json` of the other project, set the Jedlik version to `file:/absolute/path/to/jedlik/project`.
- - Publish the package to npm with the `develop` tag - `yarn publish --tag develop`. You can then install the unstable version using `yarn add @peak-ai/jednik@develop` without having to increase the version number. This is good for using the unstable version on the deployed dev environment.
