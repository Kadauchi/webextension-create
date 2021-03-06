# webextension-scripts

This package includes scripts and configuration used by [WebExtension Create](https://github.com/kadauchi/webextension-create).

##### Usage

```
webextension-scripts <script> [option]
```

##### Options

- `-v` `--version` output the version number
- `-h` `--help` output usage information

##### Commands

- `build` build folders ready for distribution
- `init [template]` initialize webextension-scripts in the current directory
- `start` start developing with auto reload

## Available Scripts

Usage:

```
npx webextension-create [options]
```

Options:
- `-v` `--version` output the version number
- `-d` `--dev` use link instead of install for webextension-scripts
- `-h` `--help` output usage information

### `npm run start`

Compiles the extension into `./build/unpacked` to be loaded into your broswer for development. The extension automatically reloads when you save changes to the code.

##### Load into Chrome

1. Open Chrome
2. Go to `chrome://extensions`
3. Turn on `Developer mode`
4. Click `Load unpacked`
5. Select folder `./build/unpacked`

##### Load into Firefox

1. Open Firefox
2. Go to `about:debugging`
3. Click `Load Temporary Add-on...`
4. Open `./build/unpacked/manifest.json`

### `npm run build`

Compiles the extension into `./build/unpacked` and then packages that into production ready zips at `./build/{target}-{version}.zip`.

### ``
