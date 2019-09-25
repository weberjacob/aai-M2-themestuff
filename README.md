# AAI M2 Theme Stuff

## For the Frontools Way.
- Add the `ashlint.js` file to the `task` directory
- Add the `ash-lint.js` file to the `helper` directory
- The `stylelint.yml` config will need to be added.
- Make sure that stylelint-order and stylelint-scss are installed using `yarn add stylelint-order stylelint-scss` when setting up Frontools
- Update `watch.js` file within SnowDog `task` directory -
  - `plugins.helper.sassLint      = require('../helper/ash-lint');`
  - remove `CSS Lint` from within `destWatcher.on('change')` -> ~ line 178
  - See `watch.js` in `Frontool Setup` for reference.

- See [August Ash 1.6](https://github.com/augustash/magento2-frontools-1.6) or [August Ash 1.7](https://github.com/augustash/magento2-frontools-1.7) for specific application and use

## Doing it directly within the Theme itself.
- **All of the following will need to be done within the root of the theme itself. For instance `src/app/design/frontend/CLIENT/THEME/`**
- Include the `config` directory along with it's contents.
- Follow the `README.md` within the `config/dev` directory for browsersync setup.
- Include the `gulpfile.js`, `package.json` and `stylelint.config.js` within the root of the theme
- Update your `config.json` file with the appropriate path for the CSS `dest`
- Run `yarn install` or `npm install` to install needed dependencies.
- Run `gulp` to watch for styling changes.
