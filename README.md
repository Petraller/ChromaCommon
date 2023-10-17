# ChromaCommon
Common HTML/JS files for Chroma Designs

* Common animation templates are in the [animations](animations) subfolder.

* Common script is used with the [ChromaDesign_Template](https://github.com/razerofficial/ChromaDesign_Template) template samples.

* Common files are also used by the [Chroma Animation Guide](https://chroma.razer.com/ChromaGuide/).


Two useful JS libraries which both use the same API referenced in the guide and should be interchangible:

* [ChromaSDKImpl.js](ChromaSDKImpl.js) - Chroma REST API Client

* [ChromaSDKWS.js](ChromaSDKWS.js) - Chroma WebSocket Client

## Usage

1. Load either `ChromaSDKImpl.js` (REST API implementation) or `ChromaSDKWS.js` (WebSocket implementation) into your web project. Both scripts should be functionally identical.

2. Call `init()` on the `chromaSDK` global object. Wait for `chromaSDK.initialized`.

3. Create, modify, and play Chroma Animations using the `ChromaAnimation` global object.

4. Shut down the Chroma SDK by calling `uninit()` on the `chromaSDK` global object.

Basic examples for using the Chroma SDK can be found in [examples](examples).

## JSDoc

JSDoc documentation for `ChromaSDKImpl.js` can be found in [docs](docs).
