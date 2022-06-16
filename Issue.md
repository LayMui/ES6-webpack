Invalid configuration object. Webpack has been initialised using a configuration object that does not match the API schema.
 - configuration.output.path: The provided value "build" is not an absolute path!
   -> The output directory as **absolute path** (required).
   

   Fix: 
   in webpack.config.js
   const path = require('path')

   entry: path.resolve(__dirname, 'app')

   Result: 
   yarn start
   you will have a build directory with bundle.js

Remove the dist directory since it's no longer needed
