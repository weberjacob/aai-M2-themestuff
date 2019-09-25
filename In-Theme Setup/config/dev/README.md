# Gulp Configuration

These files are the configuration used by our Gulp workflow. Changes **should
not** be made to config.json. If local development settings are needed,
duplicate the *example.config.local.json* and name it *config.local.json* and
make changes within that file.

Make sure to add the following to your project's `.gitignore` file.

```
/src/app/design/frontend/*/*/config/dev/config.local.json
```

```bash
$ cp example.config.local.json config.local.json
```
