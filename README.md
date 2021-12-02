# cordova-plugin-filepath

**PLEASE NOTE: This plugin is no longer actively maintained.**

This plugin allows you to resolve the native filesystem path for Android content
URIs and is based on code in the [aFileChooser](https://github.com/iPaulPro/aFileChooser/blob/master/aFileChooser/src/com/ipaulpro/afilechooser/utils/FileUtils.java) library.

Original inspiration [from StackOverflow](http://stackoverflow.com/questions/20067508/get-real-path-from-uri-android-kitkat-new-storage-access-framework).

## Installation

```bash
$ cordova plugin add cordova-plugin-filepath
```

## Supported Platforms

- Android

## Usage

Once installed the plugin defines the `window.FilePath` object. To resolve a
file path:

```js
window.FilePath.resolveNativePath(
  "content://...",
  successCallback,
  errorCallback
);
```

##### successCallback

Returns the `file://` file path.

##### errorCallback

Returns the following object:

```js
{ code: <integer>, message: <string> }
```

Possible error codes are:

- `-1` - describes an invalid action
- `0` - `file://` path could not be resolved
- `1` - the native path links to a cloud file (e.g: from Google Drive app)

## LICENSE

Apache (see LICENSE.md)

## NOTES

Support get native path from third party apps such as WhatsApp



About Android 11:		
- https://github.com/asatanasov/cordova-plugin-filepath/commit/adac021ad4e3fa5293e4dd9e44186661663896f5
- https://github.com/amacz13/cordova-plugin-filepath/commit/bf8577c916c6a9ef6dc02ffb770e9a253021261a
- https://github.com/bl1ndl3/cordova-plugin-filepath/commit/a8d4f28453c5f7f8b7fa4f24939b9bafa04cf5a7
- https://github.com/Christina1701/cordova-plugin-filepath/commit/402739ced73338f5f50783c1fb23483a707640ef
- https://github.com/denis-samodin/cordova-plugin-filepath/commit/aadebda261c8ead955dfed484ed2c2bd8048f96a error
- https://github.com/fatesinger/cordova-plugin-filepath/commit/af1dccbb59180176864f778f925762dee1cea721 lidong
- https://github.com/flobiwankenobi/cordova-plugin-filepath/commit/3526c80c91d5e3eafe7c75d775998b46020c4c23
- https://github.com/hiepnsx/cordova-plugin-filepath/commit/f098f2a7af2ee46383d8ff2b0da13bea33f1b59b  !!!
- https://github.com/humatrix-mobile/cordova-plugin-filepath/commit/dd92b2d73d37cc7d581f39861a79a32ef6c8de6f
- https://github.com/mpadmaraj/cordova-plugin-filepath/commit/e756b2a65d20a2de9884d5cfe294f30ee9e8f38f lidong
- https://github.com/MuhAssar/cordova-plugin-filepath/commit/9ace17e3c6d30338779a9bf09fb4d5293d29753f
- https://github.com/tbeata/cordova-plugin-filepath/commit/19ba5876210d5f608f6011c7316630b78af8311e
- https://github.com/tbeata/cordova-plugin-filepath/commit/19ba5876210d5f608f6011c7316630b78af8311e
- https://github.com/VIAVI-Solutions/cordova-plugin-filepath/commit/a4714209cfbd2bd8eebad902b8f5ef3e34fb8baa