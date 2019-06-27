<p align="center">
  <a href="http://ant.design">
    <img width="400" src="./assets/logo.svg">
  </a>
</p>

<!-- <h1 align="center">Dubo CLI</h1> -->

<div align="center">

POEditor cli is the Standard Tooling for workflow of POEditor.

 ![language](https://img.shields.io/badge/language-node-gcf.svg) [![npm package](https://img.shields.io/npm/v/poeditor.cli.svg?style=flat-square)](https://www.npmjs.com/package/poeditor.cli) [![NPM downloads](http://img.shields.io/npm/dm/poeditor.cli.svg?style=flat-square)](https://www.npmjs.com/package/poeditor-cli) ![license](https://img.shields.io/badge/license-Anti%20996-99ccff.svg)

</div>

## ✨ Features

- Upload pre-translated file(s) to POEditor
- Download translated files(s) to local directory

## 📦 Install

If you haven't installed [Node.js](https://nodejs.org/en/), please install it first, [here](https://nodejs.org/en/).

```bash
$ npm install poeditor.cli -g
```


## 🔨 Configuration

Create a **poeditor-config.json** in the root directory, and config information as follows:

```json
{
  "apiToken": "",                     // POEditor api token
  "projectId": 270149,                // project id
  "fileType": "android_strings",      // fileType to upload or download, supports files format (po, pot, mo, xls, csv, resw, resx, android_strings, apple_strings, xliff, properties, key_value_json, json, xmb, xtb)
  "targetDir": "./i18n"               // directory where translated files live
}
```

## 🤜🏼 Usage

Pull all translated files from upstream of POEditor.

```bash
$ poeditor pull
```

Push all pre-translated files from downloadstream of targetDir in poeditor-config.json.

```bash
$ poeditor push
```

