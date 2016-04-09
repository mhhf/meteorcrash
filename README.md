## System Info
```
Meteor 1.3.1
OS X 10.10.5
```

## Creation:
```
meteor create project
cd project
meteor npm install --save ethereumjs-testrpc
echo "import TestRPC from 'ethereumjs-testrpc';">> server/testimport.js
meteor run
```

## Observed Crash
```
[[[[[ ~/tmp/meteorcrash ]]]]]

=> Started proxy.
=> Started MongoDB.

/Users/mhhf/.meteor/packages/templating/.1.1.8.1uy9m23++os+web.browser+web.cordova/plugin.compileTemplatesBatch.os/npm/node_modules/meteor/promise/node_modules/meteor/promise/node_modules/meteor-promise/promise_server.js:116
      throw error;
            ^
TypeError: Cannot convert null to object
    at hasOwnProperty (native)
    at _.has (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:1046:27)
    at ImportScanner._resolveNodeModule (/tools/isobuild/import-scanner.js:727:9)
    at ImportScanner._tryToResolveImportedPath (/tools/isobuild/import-scanner.js:565:12)
    at ImportScanner._resolvePkgJsonMain (/tools/isobuild/import-scanner.js:812:14)
    at ImportScanner._tryToResolveImportedPath (/tools/isobuild/import-scanner.js:576:25)
    at /tools/isobuild/import-scanner.js:333:29
    at _.each._.forEach (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:87:22)
    at ImportScanner._scanFile (/tools/isobuild/import-scanner.js:332:5)
    at /tools/isobuild/import-scanner.js:399:12
    at _.each._.forEach (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:87:22)
    at ImportScanner._scanFile (/tools/isobuild/import-scanner.js:332:5)
    at /tools/isobuild/import-scanner.js:399:12
    at _.each._.forEach (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:87:22)
    at ImportScanner._scanFile (/tools/isobuild/import-scanner.js:332:5)
    at /tools/isobuild/import-scanner.js:399:12
    at _.each._.forEach (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:87:22)
    at ImportScanner._scanFile (/tools/isobuild/import-scanner.js:332:5)
    at /tools/isobuild/import-scanner.js:399:12
    at _.each._.forEach (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:87:22)
    at ImportScanner._scanFile (/tools/isobuild/import-scanner.js:332:5)
    at /tools/isobuild/import-scanner.js:399:12
    at _.each._.forEach (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:87:22)
    at ImportScanner._scanFile (/tools/isobuild/import-scanner.js:332:5)
    at /tools/isobuild/import-scanner.js:399:12
    at _.each._.forEach (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:87:22)
    at ImportScanner._scanFile (/tools/isobuild/import-scanner.js:332:5)
    at /tools/isobuild/import-scanner.js:399:12
    at _.each._.forEach (/Users/mhhf/.meteor/packages/meteor-tool/.1.3.1.2519po++os.osx.x86_64+web.browser+web.cordova/mt-os.osx.x86_64/dev_bundle/lib/node_modules/underscore/underscore.js:87:22)
    at ImportScanner._scanFile (/tools/isobuild/import-scanner.js:332:5)
    at /tools/isobuild/import-scanner.js:194:14
    at Array.forEach (native)
    at ImportScanner.scanImports (/tools/isobuild/import-scanner.js:192:22)
    at /tools/isobuild/compiler-plugin.js:791:17
    at Array.forEach (native)
    at Function.computeJsOutputFilesMap (/tools/isobuild/compiler-plugin.js:759:19)
    at ServerTarget._emitResources (/tools/isobuild/bundler.js:913:8)
    at /tools/isobuild/bundler.js:680:12
    at /tools/utils/buildmessage.js:359:18
    at [object Object].withValue (/tools/utils/fiber-helpers.js:89:14)
    at /tools/utils/buildmessage.js:352:34
    at [object Object].withValue (/tools/utils/fiber-helpers.js:89:14)
    at /tools/utils/buildmessage.js:350:23
    at [object Object].withValue (/tools/utils/fiber-helpers.js:89:14)
    at Object.enterJob (/tools/utils/buildmessage.js:324:26)
    at ServerTarget.make (/tools/isobuild/bundler.js:671:18)
    at /tools/isobuild/bundler.js:2541:14
    at /tools/isobuild/bundler.js:2609:20
    at /tools/utils/buildmessage.js:271:13
    at [object Object].withValue (/tools/utils/fiber-helpers.js:89:14)
    at /tools/utils/buildmessage.js:264:29
    at [object Object].withValue (/tools/utils/fiber-helpers.js:89:14)
    at /tools/utils/buildmessage.js:262:18
    at [object Object].withValue (/tools/utils/fiber-helpers.js:89:14)
    at /tools/utils/buildmessage.js:253:23
    at [object Object].withValue (/tools/utils/fiber-helpers.js:89:14)
    at Object.capture (/tools/utils/buildmessage.js:252:19)
    at Object.exports.bundle (/tools/isobuild/bundler.js:2493:31)
    at /tools/runners/run-app.js:591:36
    at Function.run (/tools/tool-env/profile.js:489:12)
    at bundleApp (/tools/runners/run-app.js:581:34)
    at AppRunner._runOnce (/tools/runners/run-app.js:634:35)
    at AppRunner._fiber (/tools/runners/run-app.js:887:28)
    at /tools/runners/run-app.js:411:12
```
