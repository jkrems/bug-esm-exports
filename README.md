```
$ node --experimental-modules --experimental-exports test.mjs 
(node:7866) ExperimentalWarning: The ESM module loader is experimental.
internal/modules/esm/default_resolve.js:79
  let url = moduleWrapResolve(specifier, parentURL);
            ^

Error: Cannot resolve package exports target 'undefined' matched for '.' in /home/mzasso/test/bug-exports/node_modules/my-module/package.json, imported from /home/mzasso/test/bug-exports/test.mjs
    at Loader.resolve [as _resolve] (internal/modules/esm/default_resolve.js:79:13)
    at Loader.resolve (internal/modules/esm/loader.js:73:33)
    at Loader.getModuleJob (internal/modules/esm/loader.js:152:40)
    at ModuleWrap.<anonymous> (internal/modules/esm/module_job.js:43:40)
    at link (internal/modules/esm/module_job.js:42:36) {
  code: 'ERR_MODULE_NOT_FOUND'
}
```
