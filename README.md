# @sphinx/ui-components

### This is a mono-repository which includes react-components and components-styles.

### React-components:

This package contains react-components. We're using [emotion](https://emotion.sh) to style our components. Every component has its [storybook](https://storybook.js.org) declaration.

### Components-styles:

This package contains design tokens, icons and encapsulated CSS classes, allowing the use in any JS frameworks.

## Development
1. git clone `<repo_link>`
2. yarn install
3. yarn workspaces run build  (this will build all three repositories)
4. cd packages/react-components && yarn start (this will start the storybook server)
5. yarn run lint (this will run linting)
6. yarn run test (this will run tests)

## Migration guide

### @sphinx/react-components `v6.0.0` migration
#### Update Node.js to `v16`
 - NodeJs version is increased to `v16` from `v14`. Please update your NodeJs version to `v16`. Please refer to the [official documentation](https://nodejs.org/en/download/) for the installation guide.

#### Update TypeScript to `v5.3.3`
 - TypeScript version is increased to `v5.3.3` from `v3.7.4`. Please update your TypeScript version to `v5.3.3`. Please refer to the [official documentation](https://www.typescriptlang.org/download) for the installation guide.

#### Update emotion to `v11.11.2`
 - Emotion version is increased to `v11.11.2` from `v10.0.27`. Please update your emotion version to `v11.11.2`. Please refer to the [official documentation](https://emotion.sh/docs/install) for the installation guide. Refer to the [migration guide](https://emotion.sh/docs/emotion-11) for more details.
 - Removed emotion v10 related dependencies from the package.json file.

#### Update MUI to `v5`
 - MUI version is increased to `v5` from `v4`. Please update your MUI version to `v5`. Please refer to the [official documentation](https://mui.com/getting-started/installation/) for the installation guide. Refer to the [migration guide](https://mui.com/material-ui/migration/migration-v4/) for more details.
 - MUI datepicker is updated to `v6.19.0`. Please refer to the [official documentation](https://mui.com/components/pickers/) for the installation guide.
 - As a part of the migration, we have removed the MUI v4 related dependencies from the package.json file.

#### Update react-select to `v5.8.0`
 - React-select version is increased to `v5.8.0` from `v3.0.8`. Please update your react-select version to `v5.8.0`. Please refer to the [official documentation](https://react-select.com/home) for the installation guide. Refer to the [migration guide](https://react-select.com/migration) for more details.
 - Removed react-select `v3.0.8` related dependencies from the package.json file.

### @sphinx/components-styles `v2.0.0` migration
#### Update Node.js to `v16`
 - NodeJs version is increased to `v16` from `v14`. Please update your NodeJs version to `v16`. Please refer to the [official documentation](https://nodejs.org/en/download/) for the installation guide.

#### Update TypeScript to `v5.3.3`
 - TypeScript version is increased to `v5.3.3` from `v3.7.4`. Please update your TypeScript version to `v5.3.3`. Please refer to the [official documentation](https://www.typescriptlang.org/download) for the installation guide.

#### Update emotion to `v11.11.2`
- Emotion version is increased to `v11.11.2` from `v10.0.27`. Please update your emotion version to `v11.11.2`. Please refer to the [official documentation](https://emotion.sh/docs/install) for the installation guide. Refer to the [migration guide](https://emotion.sh/docs/emotion-11) for more details on migration to `v11.11.2`.
- Removed emotion v10 related dependencies from the package.json file.

### @sphinx/tinymce-icon-pack `v4.0.0` migration
#### Update Node.js to `v16`
 - NodeJs version is increased to `v16` from `v14`. Please update your NodeJs version to `v16`. Please refer to the [official documentation](https://nodejs.org/en/download/) for the installation guide.

#### Update @sphinx/components-styles to `v2.0.0`
 - @sphinx/components-styles version is increased to `v2.0.0` from `v1`. Please update your @sphinx/components-styles version to `v2.0.0`.

## Troubleshooting
- If you face any issues while migrating to the latest version, please refer to the migration guide for the respective package. If you still face any issues, refer official documentation for migration to the latest version of the respective package.
- If you face any issue related to emotion js, make sure you should not have any emotion v10 related dependencies in your package.json file. If you have any, please remove them and install the latest version of emotion js.
- emotion js from v11 onwards, package name is changed. Please make sure you have updated the package name correctly in your code. Please refer to the [official documentation](https://emotion.sh/docs/install) for the installation guide.
- Styles applied in MUI4 and MUI5 are different. Please refer to the [official documentation](https://mui.com/guides/migration-v4/) for the migration guide from MUI4 to MUI5. We cannot use both the versions of MUI in the same project. If you are using MUI4, please refer to the migration guide and migrate to MUI5.
- From react-select v5 onwards, package is completely written in TypeScript.`@types/react-select` is not required. Please remove @types/react-select from your package.json file if you have it. In your legacy code, you might find `OptionTypeBase` interface, which is not available in the latest version. Please import `OptionTypeBase` from `@sphinx/react-component` package.     
- we are building the package using yarn workspaces. Please make sure you have installed yarn in your system. If not, please refer to the [official documentation](https://classic.yarnpkg.com/en/docs/install) for the installation guide. The package is bundled using webpack `v5` Please refer to the [official documentation](https://webpack.js.org/guides/installation/) for the installation guide.

commit 1


commit 2


commit 3


commit 4
