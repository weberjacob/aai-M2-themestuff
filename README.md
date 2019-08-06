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

## Doing it directly within the Theme itself.