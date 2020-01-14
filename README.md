# reactJS

Issue 1:

ERROR in ./main.js
Module build failed (from ./node_modules/babel-loader/lib/index.js):
Error: Cannot find module '@babel/core'
Require stack:
- C:\Users\Shubham\ReactJS\reactApp\node_modules\babel-loader\lib\index.js
- C:\Users\Shubham\ReactJS\reactApp\node_modules\loader-runner\lib\loadLoader.js
- C:\Users\Shubham\ReactJS\reactApp\node_modules\loader-runner\lib\LoaderRunner.js
- C:\Users\Shubham\ReactJS\reactApp\node_modules\webpack\lib\NormalModule.js
- C:\Users\Shubham\ReactJS\reactApp\node_modules\webpack\lib\NormalModuleFactory.js
- C:\Users\Shubham\ReactJS\reactApp\node_modules\webpack\lib\Compiler.js
- C:\Users\Shubham\ReactJS\reactApp\node_modules\webpack\lib\webpack.js
- C:\Users\Shubham\ReactJS\reactApp\node_modules\webpack-dev-server\bin\webpack-dev-server.js
 babel-loader@8 requires Babel 7.x (the package '@babel/core'). If you'd like to use Babel 6.x ('babel-core'), you should install 'babel-loader@7'.
    at Function.Module._resolveFilename (internal/modules/cjs/loader.js:973:15)
    at Function.Module._load (internal/modules/cjs/loader.js:855:27)
    at Module.require (internal/modules/cjs/loader.js:1033:19)
    at require (internal/modules/cjs/helpers.js:72:18)
    at Object.<anonymous> (C:\Users\Shubham\ReactJS\reactApp\node_modules\babel-loader\lib\index.js:10:11)
    at Module._compile (internal/modules/cjs/loader.js:1144:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:1164:10)
    at Module.load (internal/modules/cjs/loader.js:993:32)
    at Function.Module._load (internal/modules/cjs/loader.js:892:14)
    at Module.require (internal/modules/cjs/loader.js:1033:19)
 
Solution: 
npm install babel-loader @babel/core


Issue 2:
ERROR in ./main.js
Module build failed (from ./node_modules/babel-loader/lib/index.js):
Error: Cannot find module 'babel-preset-es2015' from 'C:\Users\Shubham\ReactJS\reactApp'
    at Function.module.exports [as sync] (C:\Users\Shubham\ReactJS\reactApp\node_modules\resolve\lib\sync.js:72:15)
    at resolveStandardizedName (C:\Users\Shubham\ReactJS\reactApp\node_modules\@babel\core\lib\config\files\plugins.js:101:31)
    at resolvePreset (C:\Users\Shubham\ReactJS\reactApp\node_modules\@babel\core\lib\config\files\plugins.js:58:10)
    at loadPreset (C:\Users\Shubham\ReactJS\reactApp\node_modules\@babel\core\lib\config\files\plugins.js:77:20)
    at createDescriptor (C:\Users\Shubham\ReactJS\reactApp\node_modules\@babel\core\lib\config\config-descriptors.js:154:9)
    at C:\Users\Shubham\ReactJS\reactApp\node_modules\@babel\core\lib\config\config-descriptors.js:109:50
    at Array.map (<anonymous>)
    at createDescriptors (C:\Users\Shubham\ReactJS\reactApp\node_modules\@babel\core\lib\config\config-descriptors.js:109:29)
    at createPresetDescriptors (C:\Users\Shubham\ReactJS\reactApp\node_modules\@babel\core\lib\config\config-descriptors.js:101:10)
    at C:\Users\Shubham\ReactJS\reactApp\node_modules\@babel\core\lib\config\config-descriptors.js:58:104
    
Solution:
npm install -D babel-loader @babel/preset-env webpack
 
