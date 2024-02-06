# Repo to test an issue with browserify-zlib and vite-plugin-node-polyfills

`npm run dev` to see it.

If you are at v0.18.0 or higher you should get the following (or similar) error:
```
chunk-D6GJMSXT.js?v=822e67f9:13897 Uncaught TypeError: Cannot read properties of undefined (reading 'toString')
    at node_modules/browserify-zlib/lib/index.js (chunk-D6GJMSXT.js?v=822e67f9:13897:100)
    at __require (chunk-7QXJ7KUB.js?v=822e67f9:2089:50)
    at node_modules/fast-zlib/index.js (fast-zlib.js?v=19c74098:2099:16)
    at __require (chunk-7QXJ7KUB.js?v=822e67f9:2089:50)
    at fast-zlib.js?v=19c74098:2217:16
```

If you are at v0.17.0 or less it works.
