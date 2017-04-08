# api documentation for  [cca (v0.8.1)](https://github.com/MobileChromeApps/mobile-chrome-apps#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cca.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cca) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cca.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cca)
#### Run Chrome Apps on mobile using Apache Cordova

[![NPM](https://nodei.co/npm/cca.png?downloads=true)](https://www.npmjs.com/package/cca)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cca/build/screenCapture.buildNpmdoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-cca%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cca/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cca/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cca/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "cca",
    "author": {
        "name": "The Chrome Team"
    },
    "version": "0.8.1",
    "description": "Run Chrome Apps on mobile using Apache Cordova",
    "preferGlobal": "true",
    "keywords": [
        "cordova",
        "chrome",
        "mobile",
        "apps"
    ],
    "bin": {
        "cca": "src/cca.js"
    },
    "main": "src/cca.js",
    "man": [
        "./docs/man/cca.7"
    ],
    "license": "Apache-2.0",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/MobileChromeApps/mobile-chrome-apps.git"
    },
    "dependencies": {
        "cca-manifest-logic": "^1.1.5",
        "chrome-app-developer-tool-client": "^0.0.5",
        "cordova": "^5.4.0",
        "crypto-js": "^3.1.4",
        "debounce": "^1.0.0",
        "elementtree": "0.1.6",
        "gaze": "^0.5.1",
        "node-uuid": "^1.4.1",
        "node.extend": "",
        "optimist": "~0.6.1",
        "q": "~1",
        "semver": "^4.1.0",
        "shelljs": "^0.4.0",
        "underscore": "^1.7.0",
        "update-notifier": "^0.5.0",
        "xmldom": "^0.1.19"
    },
    "files": [
        "README.md",
        "RELEASENOTES.md",
        "cordova",
        "docs",
        "src",
        "templates"
    ],
    "devDependencies": {
        "chai": "^1.9.1",
        "gulp": "^3.7.0",
        "gulp-jshint": "^1.6.1",
        "gulp-mocha": "^1.1.1",
        "gulp-util": "^3.0.1",
        "walk": "^2.3.3"
    },
    "scripts": {
        "test": "gulp test"
    },
    "bugs": {
        "url": "https://github.com/MobileChromeApps/mobile-chrome-apps/issues"
    },
    "homepage": "https://github.com/MobileChromeApps/mobile-chrome-apps#readme",
    "maintainers": [
        {
            "name": "agrieve",
            "email": "agrieve@chromium.org"
        },
        {
            "name": "mmocny",
            "email": "mmocny@gmail.com"
        },
        {
            "name": "shepheb",
            "email": "braden.shepherdson@gmail.com"
        },
        {
            "name": "maxw",
            "email": "maxw@chromium.org"
        },
        {
            "name": "clelland",
            "email": "iclelland@google.com"
        },
        {
            "name": "kamrik",
            "email": "kamrik@gmail.com"
        },
        {
            "name": "drkemp",
            "email": "drkemp@chromium.org"
        }
    ],
    "dist": {
        "shasum": "9bc7a526b5e8f638a46ff994f8258731970a2caa",
        "tarball": "https://registry.npmjs.org/cca/-/cca-0.8.1.tgz"
    },
    "directories": {},
    "readme": "ERROR: No README data found!"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cca](#apidoc.module.cca)
1.  [function <span class="apidocSignatureSpan">cca.</span>parseCLI ()](#apidoc.element.cca.parseCLI)
1.  [function <span class="apidocSignatureSpan">cca.</span>tools_check ()](#apidoc.element.cca.tools_check)
1.  object <span class="apidocSignatureSpan">cca.</span>analytics
1.  object <span class="apidocSignatureSpan">cca.</span>analytics_loader
1.  object <span class="apidocSignatureSpan">cca.</span>cordova_commands
1.  object <span class="apidocSignatureSpan">cca.</span>hooks
1.  object <span class="apidocSignatureSpan">cca.</span>upgrade_project
1.  object <span class="apidocSignatureSpan">cca.</span>utils

#### [module cca.analytics](#apidoc.module.cca.analytics)
1.  [function <span class="apidocSignatureSpan">cca.analytics.</span>sendEvent (eventCategory, eventAction)](#apidoc.element.cca.analytics.sendEvent)

#### [module cca.analytics_loader](#apidoc.module.cca.analytics_loader)
1.  [function <span class="apidocSignatureSpan">cca.analytics_loader.</span>analyticsCommand (command)](#apidoc.element.cca.analytics_loader.analyticsCommand)
1.  [function <span class="apidocSignatureSpan">cca.analytics_loader.</span>getAnalyticsModule (useTestingVersion)](#apidoc.element.cca.analytics_loader.getAnalyticsModule)
1.  [function <span class="apidocSignatureSpan">cca.analytics_loader.</span>readWriteUserConfig (userConfig)](#apidoc.element.cca.analytics_loader.readWriteUserConfig)

#### [module cca.cordova_commands](#apidoc.module.cca.cordova_commands)
1.  [function <span class="apidocSignatureSpan">cca.cordova_commands.</span>runAllCmds (commands)](#apidoc.element.cca.cordova_commands.runAllCmds)
1.  [function <span class="apidocSignatureSpan">cca.cordova_commands.</span>runCmd (cmd)](#apidoc.element.cca.cordova_commands.runCmd)

#### [module cca.hooks](#apidoc.module.cca.hooks)
1.  [function <span class="apidocSignatureSpan">cca.hooks.</span>beforePluginAdd (context)](#apidoc.element.cca.hooks.beforePluginAdd)
1.  [function <span class="apidocSignatureSpan">cca.hooks.</span>postPrepare (opts)](#apidoc.element.cca.hooks.postPrepare)
1.  [function <span class="apidocSignatureSpan">cca.hooks.</span>prePrepare (context)](#apidoc.element.cca.hooks.prePrepare)
1.  [function <span class="apidocSignatureSpan">cca.hooks.</span>registerHooks ()](#apidoc.element.cca.hooks.registerHooks)
1.  [function <span class="apidocSignatureSpan">cca.hooks.</span>unregisterHooks ()](#apidoc.element.cca.hooks.unregisterHooks)

#### [module cca.tools_check](#apidoc.module.cca.tools_check)
1.  [function <span class="apidocSignatureSpan">cca.</span>tools_check ()](#apidoc.element.cca.tools_check.tools_check)
1.  [function <span class="apidocSignatureSpan">cca.tools_check.</span>fixEnv ()](#apidoc.element.cca.tools_check.fixEnv)

#### [module cca.upgrade_project](#apidoc.module.cca.upgrade_project)
1.  [function <span class="apidocSignatureSpan">cca.upgrade_project.</span>upgradeProject (skipPrompt)](#apidoc.element.cca.upgrade_project.upgradeProject)
1.  [function <span class="apidocSignatureSpan">cca.upgrade_project.</span>upgradeProjectIfStale (skipPrompt)](#apidoc.element.cca.upgrade_project.upgradeProjectIfStale)

#### [module cca.utils](#apidoc.module.cca.utils)
1.  [function <span class="apidocSignatureSpan">cca.utils.</span>assetDirForPlatform (platform)](#apidoc.element.cca.utils.assetDirForPlatform)
1.  [function <span class="apidocSignatureSpan">cca.utils.</span>colorizeConsole ()](#apidoc.element.cca.utils.colorizeConsole)
1.  [function <span class="apidocSignatureSpan">cca.utils.</span>exec (cmd, opt_silent)](#apidoc.element.cca.utils.exec)
1.  [function <span class="apidocSignatureSpan">cca.utils.</span>exit (code)](#apidoc.element.cca.utils.exit)
1.  [function <span class="apidocSignatureSpan">cca.utils.</span>fatal (msg)](#apidoc.element.cca.utils.fatal)
1.  [function <span class="apidocSignatureSpan">cca.utils.</span>fixPathSlashes (p)](#apidoc.element.cca.utils.fixPathSlashes)
1.  [function <span class="apidocSignatureSpan">cca.utils.</span>isWindows ()](#apidoc.element.cca.utils.isWindows)
1.  [function <span class="apidocSignatureSpan">cca.utils.</span>waitForKey (opt_prompt)](#apidoc.element.cca.utils.waitForKey)



# <a name="apidoc.module.cca"></a>[module cca](#apidoc.module.cca)

#### <a name="apidoc.element.cca.parseCLI"></a>[function <span class="apidocSignatureSpan">cca.</span>parseCLI ()](#apidoc.element.cca.parseCLI)
- description and source-code
```javascript
function main() {
  cordovaLib.binname = 'cca';

  var commandLineFlags = require('./parse-command-line')();
  utils.exit.pause_on_exit = commandLineFlags.pause_on_exit;

  // TODO: Should we support an opt out '--no-update-notifier'?
  var pkg = require('../package.json');
  updateNotifier({
    pkg: pkg,
    updateCheckInterval: 1000 * 60 * 60 * 24, // Daily
  }).notify();

  var command = commandLineFlags._[0];
  var packageVersion = require('../package').version;

  // Colorize after parseCommandLine to avoid --help being printed in red.
  utils.colorizeConsole();

  hooks.registerHooks();

  function printCcaVersionPrefix() {
    console.log('cca v' + packageVersion);
  }

  if (command == 'exec') {
    return require('./tools-check').fixEnv()
    .then(function() {
      require('./exec')(process.argv.slice(3));
    }).done(null, utils.fatal);
  }

  if (commandLineFlags.v) {
    command = 'version';
  }
  if (commandLineFlags.h || !command) {
    command = 'help';
  }

  function autoAddPlatforms() {
    var plats = [];
    if (process.argv.indexOf('android') != -1 && !fs.existsSync(path.join('platforms', 'android'))) {
      plats.push('android');
    }
    if (process.argv.indexOf('ios') != -1 && !fs.existsSync(path.join('platforms', 'ios'))) {
      plats.push('ios');
    }
    if (plats.length === 0) {
      return Q();
    }
    var argv = require('optimist')
        .options('link', { type: 'boolean' })
        .options('verbose', { type: 'boolean', alias: 'd' })
        .argv;
    var opts = {
      link: argv.link,
      verbose: argv.verbose
    };
    return require('./cordova-commands').runCmd(['platform', 'add', plats, opts])
    .then(require('./write-out-cca-version'));
  }

  function beforeCordovaPrepare() {
    return autoAddPlatforms()
    .then(function() {
      if (commandLineFlags['skip-upgrade']) {
        return;
      }
      if (!fs.existsSync(path.join('www', 'manifest.json'))) {
        return Q.reject('This is not a cca project (no www/manifest.json file). Perhaps you meant to use the cordova-cli?');
      }
      return require('./upgrade-project').upgradeProjectIfStale(commandLineFlags.y);
    });
  }

  function forwardCurrentCommandToCordova() {
    // Unregister some event handlers in cordova-lib EventEmitter. Otherwise
    // double printouts will happen because cordova-cli registers its own
    // handlers. This is only relevant when --verbose or -d flag is used.
    cordovaLib.events.removeListener('results', console.log);
    cordovaLib.events.removeListener('log', console.log);
    cordovaLib.events.removeListener('warn', console.warn);
    cordovaLib.events.removeListener('verbose', console.log);

    // TODO: Can we replace use of CLI here?  Calls to cordova-lib cordova.raw?
    return cordova.cli(process.argv);
  }

  function printVersionThenPrePrePrepareThenForwardCommandToCordova() {
    printCcaVersionPrefix();
    return beforeCordovaPrepare()
      .then(forwardCurrentCommandToCordova);
  }

  var commandActions = {
    'pre-prepare': function() {
      return require('./pre-prepare')();
    },
    'update-app': function() {
      // TODO: deprecated command, use post-prepare instead
      return commandActions['post-prepare']();
    },
    'post-prepare': function() {
      return require('./post-prepare')();
    },
    'checkenv': function() {
      printCcaVersionPrefix();
      return require('./tools-check')();
    },
    'push': function() {
      printCcaVersionPrefix();
      return Q.fcall(function() {
        var extraFlag = commandLineFlags._[1] || '';
        if (extraFlag) {
          require('optimist').showHelp(console.log);
          return Q.reject('Flag "' + extraFlag + '" not understood.  Did you mean '--target=' + extraFlag + ''?');
        }
        return require('./push-to-harness')(commandLineFlags.target, commandLineFlags.watch);
      });
    },
    'run': function() {
      printCcaVersionPrefix();
      var platform = commandLineFlags._[1];
      if (platform === 'chrome' || platform === 'canary') {
        return require('./run-in-chrome' ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.tools_check"></a>[function <span class="apidocSignatureSpan">cca.</span>tools_check ()](#apidoc.element.cca.tools_check)
- description and source-code
```javascript
function toolsCheck() {
  var ret = Q();

  // Is this the first time we're checking for the tools?
  if (typeof hasAndroidPlatform == 'undefined') {
    ret = ret.then(function() {
      return checkHasAndroid().then(checkHasIos);
    });
  }

  return ret.then(function() {
    if (!hasAndroidPlatform && !hasXcode)
      // TODO: Replace inline docs links with general instructions to read --help / docs / report issues
      return Q.reject('No usable build environment could be found. Please refer to our installation guide:\n' +
          'https://github.com/MobileChromeApps/mobile-chrome-apps/blob/master/docs/Installation.md');

    return Q({
      hasAndroidPlatform: hasAndroidPlatform,
      hasXcode: hasXcode,
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cca.analytics"></a>[module cca.analytics](#apidoc.module.cca.analytics)

#### <a name="apidoc.element.cca.analytics.sendEvent"></a>[function <span class="apidocSignatureSpan">cca.analytics.</span>sendEvent (eventCategory, eventAction)](#apidoc.element.cca.analytics.sendEvent)
- description and source-code
```javascript
sendEvent = function (eventCategory, eventAction) {
  var url = URL_BASE;
  url += '&t=event';
  url += '&ec=' + eventCategory;
  url += '&ea=' + eventAction;

  sendMeasurement(url);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cca.analytics_loader"></a>[module cca.analytics_loader](#apidoc.module.cca.analytics_loader)

#### <a name="apidoc.element.cca.analytics_loader.analyticsCommand"></a>[function <span class="apidocSignatureSpan">cca.analytics_loader.</span>analyticsCommand (command)](#apidoc.element.cca.analytics_loader.analyticsCommand)
- description and source-code
```javascript
function analyticsCommand(command) {
  var usage = ''cca analytics [enable|disable]'';

  // 'cca analytics' will tell the user whether analytics are enabled or disabled.
  if (!command) {
    var userConfig = readWriteUserConfig();
    var permission = userConfig && userConfig.analytics && userConfig.analytics.isAllowed;
    var outputText = 'Usage statistics collection is currently ' + (permission ? 'enabled' : 'disabled') + '. ';
    outputText += 'To change this, run ' + usage + '.';
    console.log(outputText);
    return;
  }

  // We only allow 'enable' and 'disable'; print an error if we were given something else.
  command = command.toLowerCase();
  if (command != 'enable' && command != 'disable') {
    var errorText = 'Invalid argument: ' + command + '. ';
    errorText += 'To enable or disable usage statistics collection, run ' + usage + '.';
    utils.fatal(errorText);
    return;
  }

  // Set analytics permission according to the given command.
  writePermission(command == 'enable');
  console.log('Usage statistics collection ' + command + 'd.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.analytics_loader.getAnalyticsModule"></a>[function <span class="apidocSignatureSpan">cca.analytics_loader.</span>getAnalyticsModule (useTestingVersion)](#apidoc.element.cca.analytics_loader.getAnalyticsModule)
- description and source-code
```javascript
function getAnalyticsModule(useTestingVersion) {
  if (useTestingVersion) {
    analyticsModule = makeFakeModule(true /* logCalls */);
    return Q(analyticsModule);
  }

  // If we've already loaded an analytics module, use the one we already have.
  if (analyticsModule) {
    return Q(analyticsModule);
  }

  // Ask for permission and return a module accordingly.
  return requestPermission()
  .then(function(permission) {
    analyticsModule = permission ? require('./analytics') : makeFakeModule(false /* logCalls */);
    return Q(analyticsModule);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.analytics_loader.readWriteUserConfig"></a>[function <span class="apidocSignatureSpan">cca.analytics_loader.</span>readWriteUserConfig (userConfig)](#apidoc.element.cca.analytics_loader.readWriteUserConfig)
- description and source-code
```javascript
function readWriteUserConfig(userConfig) {
  // Determine the path of the config file.
  // We use this format to comply with the 'rc' config loader (https://github.com/dominictarr/rc), in case we use that in the future
.
  var HOME = process.env[(process.platform.slice(0, 3) == 'win') ? 'USERPROFILE' : 'HOME'];
  var userConfigDir = path.join(HOME, '.cca');
  var userConfigPath = path.join(userConfigDir, 'config');

  // Write to the file if we were passed an argument, or read and return it if we were.
  // If we were instructed to read the file, but it doesn't exist, return null.
  if (userConfig) {
    shelljs.mkdir('-p', userConfigDir);
    fs.writeFileSync(userConfigPath, JSON.stringify(userConfig, null, 4));
  } else if (fs.existsSync(userConfigPath)) {
    userConfig = JSON.parse(fs.readFileSync(userConfigPath, 'utf-8'));
    return userConfig;
  } else {
    return null;
  }
}
```
- example usage
```shell
...
URL_BASE += '&cid=' + cid;
URL_BASE += '&an=' + an;
URL_BASE += '&av=' + av;

// This function retrieves the client ID from the config file or generates if it one doesn't exist.
function getClientId() {
var analyticsLoader = require('./analytics-loader');
var userConfig = analyticsLoader.readWriteUserConfig();

// Return the client id from the file, if one is there.
if (userConfig && userConfig.analytics && userConfig.analytics.clientId) {
  return userConfig.analytics.clientId;
}

// We don't have a client id yet, so generate one, save it, and return it.
...
```



# <a name="apidoc.module.cca.cordova_commands"></a>[module cca.cordova_commands](#apidoc.module.cca.cordova_commands)

#### <a name="apidoc.element.cca.cordova_commands.runAllCmds"></a>[function <span class="apidocSignatureSpan">cca.cordova_commands.</span>runAllCmds (commands)](#apidoc.element.cca.cordova_commands.runAllCmds)
- description and source-code
```javascript
function runAllCmds(commands) {
  return commands.reduce(function(soFar, f) {
    return soFar.then(function() {
      return exports.runCmd(f);
    });
  }, Q());
}
```
- example usage
```shell
...
  var cmds = [];
  if (flags.ios) {
    cmds.push(['platform', 'add', 'ios']);
  }
  if (flags.android) {
    cmds.push(['platform', 'add', 'android']);
  }
  return require('./cordova-commands').runAllCmds(cmds);
})
.then(function() {
  var wwwPath = path.join(destAppDir, 'www');
  var welcomeText = 'Done!\n\n';
  if (flags['link-to']) {
    welcomeText += 'Your project has been created, with web assets symlinked to the following chrome app:\n' +
                   wwwPath + ' --> ' + srcAppDir + '\n\n';
...
```

#### <a name="apidoc.element.cca.cordova_commands.runCmd"></a>[function <span class="apidocSignatureSpan">cca.cordova_commands.</span>runCmd (cmd)](#apidoc.element.cca.cordova_commands.runCmd)
- description and source-code
```javascript
function runCmd(cmd) {
  var msg = cmd[0];
  cmd.slice(1).forEach(function(arg) {
    if (Array.isArray(arg)) {
      msg += ' ' + arg.join(' ');
      return;
    } else if (typeof arg != 'string') {
      return;
    }
    if (arg.indexOf(' ') != -1) {
      msg += ' "' + arg + '"';
    } else {
      msg += ' ' + arg;
    }
  });
  console.log('## Running Cordova Command: ' + msg);
  return cordova.raw[cmd[0]].apply(cordova, cmd.slice(1));
}
```
- example usage
```shell
...
  return cordova.raw[cmd[0]].apply(cordova, cmd.slice(1));
};

// Chains a list of cordova commands, returning a promise.
exports.runAllCmds = function runAllCmds(commands) {
  return commands.reduce(function(soFar, f) {
    return soFar.then(function() {
      return exports.runCmd(f);
    });
  }, Q());
};
...
```



# <a name="apidoc.module.cca.hooks"></a>[module cca.hooks](#apidoc.module.cca.hooks)

#### <a name="apidoc.element.cca.hooks.beforePluginAdd"></a>[function <span class="apidocSignatureSpan">cca.hooks.</span>beforePluginAdd (context)](#apidoc.element.cca.hooks.beforePluginAdd)
- description and source-code
```javascript
function beforePluginAdd(context) {
  return getManifest('www')
    .then(function(manifest) {
      return ccaManifestLogic.analyseManifest(manifest);
    })
    .then(function(manifestData) {
      var pluginsToBeNotInstalled = manifestData.pluginsToBeNotInstalled.concat();
      var pluginsBeingInstalledRightNow = context.plugins;

      pluginsToBeNotInstalled = pluginsToBeNotInstalled.filter(function(plugin) {
        return pluginsBeingInstalledRightNow.indexOf(plugin) != -1;
      });

      if (pluginsToBeNotInstalled.length === 0) return;

      console.error("Error: The following plugin(s) cannot be explicitly installed:");
      pluginsToBeNotInstalled.forEach(function(plugin) {
        console.warn("*", plugin);
      });
      console.error("Instead, add the proper manifest.json permissions.");
      console.error("See: https://developer.chrome.com/apps/manifest");

      return Q.reject("Abort plugin add");
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.hooks.postPrepare"></a>[function <span class="apidocSignatureSpan">cca.hooks.</span>postPrepare (opts)](#apidoc.element.cca.hooks.postPrepare)
- description and source-code
```javascript
function postPrepareCommand(opts) {
  var hasAndroid = fs.existsSync(path.join('platforms', 'android'));
  var hasIos = fs.existsSync(path.join('platforms', 'ios'));

  if (!fs.existsSync('platforms')) {
    return Q.reject('No platforms directory found. Please run script from the root of your project.');
  }

  var p = Q();
  if (hasAndroid) {
    p = p.then(function() { return postPrepareInternal('android'); });
  }
  if (hasIos) {
    p = p.then(function() { return postPrepareInternal('ios'); });
  }
  return p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.hooks.prePrepare"></a>[function <span class="apidocSignatureSpan">cca.hooks.</span>prePrepare (context)](#apidoc.element.cca.hooks.prePrepare)
- description and source-code
```javascript
function prePrepareCommand(context) {
  // context is the Context object passed in by cordova-lib/HooksRunner.
  var pluginsToBeInstalled = [];
  var pluginsToBeNotInstalled = [];
  var pluginsNotRecognized = [];
  var manifest, whitelist;
  // Convert all plugin IDs to lower case (registry has problems with upper case).
  var installedPlugins = context.cordova.plugins.map(function(s) { return s.toLowerCase(); });

  var argv = require('optimist')
      .options('webview', { type: 'string' })
      .options('release', { type: 'boolean' })
      .options('link', { type: 'boolean' })
      .options('verbose', { type: 'boolean', alias: 'd' })
      .argv;

  // Pre-prepare manifest check and project munger
  return require('./get-manifest')('www')
  .then(function(m) {
    manifest = m;
    if (argv.webview) {
        manifest.webview = argv.webview;
    }

    return ccaManifestLogic.analyseManifest(manifest);
  })
  .then(function(manifestData) {
    pluginsToBeInstalled = manifestData.pluginsToBeInstalled.concat(['org.chromium.cca-hooks']);
    pluginsToBeNotInstalled = manifestData.pluginsToBeNotInstalled.concat();
    pluginsNotRecognized = manifestData.pluginsNotRecognized;
    whitelist = manifestData.whitelist;

    var configXmlData = fs.readFileSync('config.xml', 'utf8');
    var configXmlDom = new xmldom.DOMParser().parseFromString(configXmlData);
    ccaManifestLogic.updateConfigXml(manifest, manifestData, configXmlDom);
    var newConfigData = new xmldom.XMLSerializer().serializeToString(configXmlDom);
    // Don't write out if nothing actually changed
    if (newConfigData != configXmlData) {
      console.log('## Updating config.xml from manifest.json');
      fs.writeFileSync('config.xml', newConfigData);
    }
  })
  .then(function() {
    if ( (context.cordova.platforms.indexOf('android') != -1) && argv['release']) {
      if (!fs.existsSync('android-release-keys.properties')) {
        utils.fatal('Cannot build android in release mode: android-release-keys.properties not found in project root.');
      }
    }
    // Add a URL type to the iOS project's .plist file.
    // This is necessary for chrome.identity to redirect back to the app after authentication.
    var hasIos = fs.existsSync(path.join('platforms', 'ios'));
    if (hasIos) {
      var platforms = cordovaLib.cordova_platforms;
      var parser = platforms.getPlatformApi('ios');
      var infoPlistPath = path.join('platforms', 'ios', parser._parser.originalName, parser._parser.originalName + '-Info.plist');
      var infoPlistXml = et.parse(fs.readFileSync(infoPlistPath, 'utf-8'));

      var rootPlistElement = infoPlistXml.getroot();
      var rootDictElement = rootPlistElement.getItem(0);

      var bundleUrlTypesKey = et.SubElement(rootDictElement, 'key');
      bundleUrlTypesKey.text = 'CFBundleURLTypes';
      var bundleUrlTypesArray = et.SubElement(rootDictElement, 'array');
      var bundleUrlTypesDict = et.SubElement(bundleUrlTypesArray, 'dict');

      var bundleTypeRoleKey = et.SubElement(bundleUrlTypesDict, 'key');
      bundleTypeRoleKey.text = 'CFBundleTypeRole';
      var bundleTypeRoleString = et.SubElement(bundleUrlTypesDict, 'string');
      bundleTypeRoleString.text = 'Editor';

      var bundleUrlNameKey = et.SubElement(bundleUrlTypesDict, 'key');
      bundleUrlNameKey.text = 'CFBundleURLName';
      var bundleUrlNameString = et.SubElement(bundleUrlTypesDict, 'string');
      bundleUrlNameString.text = manifest.packageId;

      var bundleUrlSchemesKey = et.SubElement(bundleUrlTypesDict, 'key');
      bundleUrlSchemesKey.text = 'CFBundleURLSchemes';
      var bundleUrlSchemesArray = et.SubElement(bundleUrlTypesDict, 'array');
      var bundleUrlSchemeString = et.SubElement(bundleUrlSchemesArray, 'string');
      bundleUrlSchemeString.text = manifest.packageId;

      fs.writeFileSync(infoPlistPath, infoPlistXml.write({indent: 4}), 'utf-8');
    }
  })
  .then(function() {
    var missingPlugins = __.difference(pluginsToBeInstalled, installedPlugins);
    var excessPlugins = __.intersection(installedPlugins, pluginsToBeNotIns ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.hooks.registerHooks"></a>[function <span class="apidocSignatureSpan">cca.hooks.</span>registerHooks ()](#apidoc.element.cca.hooks.registerHooks)
- description and source-code
```javascript
function registerHooks() {
  cordovaLib.events.on('before_prepare', prePrepare);
  cordovaLib.events.on('after_prepare', postPrepare);
  cordovaLib.events.on('before_plugin_add', beforePluginAdd);
}
```
- example usage
```shell
...
      };
      return require('./cordova-commands').runCmd(['platform', 'add', plats, opts]);
    }
  })
  .then(function() {
    // Turn the hooks back on and fire prepare. The pre-prepare hook is what
    // installs all the cca plugins back.
    hooks.registerHooks();
    return cordova.raw.prepare();
  })
  .then(require('./write-out-cca-version'));
}
...
```

#### <a name="apidoc.element.cca.hooks.unregisterHooks"></a>[function <span class="apidocSignatureSpan">cca.hooks.</span>unregisterHooks ()](#apidoc.element.cca.hooks.unregisterHooks)
- description and source-code
```javascript
function unregisterHooks() {
  cordovaLib.events.removeListener('before_prepare', prePrepare);
  cordovaLib.events.removeListener('after_prepare', postPrepare);
  cordovaLib.events.removeListener('before_plugin_add', beforePluginAdd);
}
```
- example usage
```shell
...
  return Q.reject('Okay, nevermind.');
}
  })
  .then(function() {
// Upgrading!

// We don't want the pre/post prepare hooks to fire during upgrade.
hooks.unregisterHooks();

// Remove the old file based pre/post prepare hooks
// TODO: Remove this later. Last version to use file based hooks was 4.0.0 released in Oct 2014.
shelljs.rm('-f', path.join('hooks', 'before_prepare', 'cca-pre-prepare.js'));
shelljs.rm('-f', path.join('hooks', 'after_prepare', 'cca-post-prepare.js'));

// Remember what platforms we had before deleting them. If we only had one, don't install the other after upgrade.
...
```



# <a name="apidoc.module.cca.tools_check"></a>[module cca.tools_check](#apidoc.module.cca.tools_check)

#### <a name="apidoc.element.cca.tools_check.tools_check"></a>[function <span class="apidocSignatureSpan">cca.</span>tools_check ()](#apidoc.element.cca.tools_check.tools_check)
- description and source-code
```javascript
function toolsCheck() {
  var ret = Q();

  // Is this the first time we're checking for the tools?
  if (typeof hasAndroidPlatform == 'undefined') {
    ret = ret.then(function() {
      return checkHasAndroid().then(checkHasIos);
    });
  }

  return ret.then(function() {
    if (!hasAndroidPlatform && !hasXcode)
      // TODO: Replace inline docs links with general instructions to read --help / docs / report issues
      return Q.reject('No usable build environment could be found. Please refer to our installation guide:\n' +
          'https://github.com/MobileChromeApps/mobile-chrome-apps/blob/master/docs/Installation.md');

    return Q({
      hasAndroidPlatform: hasAndroidPlatform,
      hasXcode: hasXcode,
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.tools_check.fixEnv"></a>[function <span class="apidocSignatureSpan">cca.tools_check.</span>fixEnv ()](#apidoc.element.cca.tools_check.fixEnv)
- description and source-code
```javascript
fixEnv = function () {
  return check_reqs.check_java()
  .then(function() {
    return check_reqs.check_android();
  })
  .then(null, function() {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cca.upgrade_project"></a>[module cca.upgrade_project](#apidoc.module.cca.upgrade_project)

#### <a name="apidoc.element.cca.upgrade_project.upgradeProject"></a>[function <span class="apidocSignatureSpan">cca.upgrade_project.</span>upgradeProject (skipPrompt)](#apidoc.element.cca.upgrade_project.upgradeProject)
- description and source-code
```javascript
function upgradeProject(skipPrompt) {
  var argv = require('optimist')
      .options('link', { type: 'boolean' })
      .options('verbose', { type: 'boolean', alias: 'd' })
      .argv;
  var hadPlatforms = [];

  return Q()
  .then(function(){
    if (skipPrompt) return 'y';
    return utils.waitForKey('Warning: Upgrade will replace all files in platforms and plugins. Continue? [y/N] ');
  })
  .then(function(key) {
    if (key != 'y' && key != 'Y') {
      return Q.reject('Okay, nevermind.');
    }
  })
  .then(function() {
    // Upgrading!

    // We don't want the pre/post prepare hooks to fire during upgrade.
    hooks.unregisterHooks();

    // Remove the old file based pre/post prepare hooks
    // TODO: Remove this later. Last version to use file based hooks was 4.0.0 released in Oct 2014.
    shelljs.rm('-f', path.join('hooks', 'before_prepare', 'cca-pre-prepare.js'));
    shelljs.rm('-f', path.join('hooks', 'after_prepare', 'cca-post-prepare.js'));

    // Remember what platforms we had before deleting them. If we only had one, don't install the other after upgrade.
    hadPlatforms = getInstalledPlatfroms();
    shelljs.rm('-rf', 'platforms');

    shelljs.rm('-f', path.join('plugins', 'android.json'));
    shelljs.rm('-f', path.join('plugins', 'ios.json'));

    var installedPlugins = cordova.cordova_lib.PluginInfo.loadPluginsDir('plugins');
    installedPlugins = __.pluck(installedPlugins, 'id');

    // Only remove the CCA managed plugins
    var allCcaPlugins = getCcaPlugins();
    var pluginsToRemove = __.intersection(allCcaPlugins, installedPlugins);
    if (pluginsToRemove && pluginsToRemove.length) {
      return require('./cordova-commands').runCmd(['plugin', 'rm', pluginsToRemove]);
    }
  })
  .then(function() {
    console.log('## First-time build. Detecting available SDKs:');
    return getSupportedPlatforms();
  })
  .then(function(plats) {
    if (plats.length) {
      // If this is a real upgrade, only install the platforms we had before.
      if (hadPlatforms.length) {
        plats = __.intersection(plats, hadPlatforms);
      }
      var opts = {
        link: argv.link,
        verbose: argv.verbose
      };
      return require('./cordova-commands').runCmd(['platform', 'add', plats, opts]);
    }
  })
  .then(function() {
    // Turn the hooks back on and fire prepare. The pre-prepare hook is what
    // installs all the cca plugins back.
    hooks.registerHooks();
    return cordova.raw.prepare();
  })
  .then(require('./write-out-cca-version'));
}
```
- example usage
```shell
...
  var installedPlatfroms = getInstalledPlatfroms();

  if (!installedPlatfroms.length) {
// No platforms installed yet, (ab)use upgradeProject(skipPrompt=true) to install both.
// Ideally we would do this in pre-prepare, but cordova doesn't run pre-prepare scripts if there
// are no target platforms, and its unclear how to make it do so with a difference concept
// for pre-prepare scripts.
return exports.upgradeProject(true);
  } else {

var versionFile = path.join('platforms', 'created-with-cca-version');
var createdWith;
if (fs.existsSync(versionFile)) {
  createdWith = fs.readFileSync(versionFile, 'utf-8').trim();
}
...
```

#### <a name="apidoc.element.cca.upgrade_project.upgradeProjectIfStale"></a>[function <span class="apidocSignatureSpan">cca.upgrade_project.</span>upgradeProjectIfStale (skipPrompt)](#apidoc.element.cca.upgrade_project.upgradeProjectIfStale)
- description and source-code
```javascript
function upgradeProjectIfStale(skipPrompt) {
  var packageVersion = require('../package').version;
  var installedPlatfroms = getInstalledPlatfroms();

  if (!installedPlatfroms.length) {
    // No platforms installed yet, (ab)use upgradeProject(skipPrompt=true) to install both.
    // Ideally we would do this in pre-prepare, but cordova doesn't run pre-prepare scripts if there
    // are no target platforms, and its unclear how to make it do so with a difference concept
    // for pre-prepare scripts.
    return exports.upgradeProject(true);
  } else {

    var versionFile = path.join('platforms', 'created-with-cca-version');
    var createdWith;
    if (fs.existsSync(versionFile)) {
      createdWith = fs.readFileSync(versionFile, 'utf-8').trim();
    }
    if (createdWith == packageVersion) {
      return Q();
    } else {
      // The platforms/created-with-cca-version file does not exist or contains older version string. Upgrading.
      console.log('This project was not upgraded to cca v' + packageVersion + ' yet.  Attempting to upgrade now...');
      return exports.upgradeProject(skipPrompt);
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cca.utils"></a>[module cca.utils](#apidoc.module.cca.utils)

#### <a name="apidoc.element.cca.utils.assetDirForPlatform"></a>[function <span class="apidocSignatureSpan">cca.utils.</span>assetDirForPlatform (platform)](#apidoc.element.cca.utils.assetDirForPlatform)
- description and source-code
```javascript
function assetDirForPlatform(platform) {
  if (platform === 'android') {
    return path.join('platforms', platform, 'assets','www');
  }
  return path.join('platforms', platform, 'www');
}
```
- example usage
```shell
...
var html = fs.readFileSync(htmlPath, 'utf8');
html = html.replace(/<meta.*Content-Security.*>/, cspTag);
fs.writeFileSync(htmlPath, html);
}

// Internal function called potentially multiple times to cover all platforms.
function postPrepareInternal(platform) {
var root = utils.assetDirForPlatform(platform);
var localesPath = path.join(utils.assetDirForPlatform(platform), '_locales');
return Q().then(function() {
  if (!fs.existsSync(localesPath)) {
    return;
  }
  console.log('## Normalizing _locales for ' + platform);
  return Q.ninvoke(fs, 'readdir', localesPath)
...
```

#### <a name="apidoc.element.cca.utils.colorizeConsole"></a>[function <span class="apidocSignatureSpan">cca.utils.</span>colorizeConsole ()](#apidoc.element.cca.utils.colorizeConsole)
- description and source-code
```javascript
function colorizeConsole() {
  var origWarn = console.warn;
  console.warn = function() {
    var msg = [].slice.call(arguments).join(' ');
    origWarn.call(console, '\x1B[33m' + msg + '\x1B[39m');
  };
  console.error = function() {
    var msg = [].slice.call(arguments).join(' ');
    origWarn.call(console, '\x1B[31m' + msg + '\x1B[39m');
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.utils.exec"></a>[function <span class="apidocSignatureSpan">cca.utils.</span>exec (cmd, opt_silent)](#apidoc.element.cca.utils.exec)
- description and source-code
```javascript
function exec(cmd, opt_silent) {
  if (!opt_silent) {
    console.log('Running: ' + cmd);
  }
  var d = Q.defer();
  childProcess.exec(cmd, function(error, stdout, stderr) {
    if (error) {
      d.reject(error);
    } else {
      d.resolve({
        stdout: stdout.trim(),
        stderr: stderr.trim()
      });
    }
  });
  return d.promise;
}
```
- example usage
```shell
...
}

function checkFileHandleLimit() {
var deferred = Q.defer();
if (process.platform != 'win32' && process.env['SHELL']) {
  // gaze opens a lot of file handles, and the default on OS X is too small (EMFILE exceptions).
  // NOTE: This is fixed in node 0.11, and is a problem only on node 0.10.
  child_process.exec('ulimit -n', function(error, stdout, stderr) {
    var curLimit = !error && +stdout;
    deferred.resolve(curLimit || Infinity);
  });
} else {
  deferred.resolve(Infinity);
}
return deferred.promise;
...
```

#### <a name="apidoc.element.cca.utils.exit"></a>[function <span class="apidocSignatureSpan">cca.utils.</span>exit (code)](#apidoc.element.cca.utils.exit)
- description and source-code
```javascript
function exit(code) {
  if (exports.exit.pause_on_exit) {
    exports.waitForKey(function() {
      process.exit(code);
    });
  } else {
    process.exit(code);
  }
}
```
- example usage
```shell
...
function writeHook(path) {
  var contents = [
      "#!/usr/bin/env node",
      "var cmdline = process.env['CORDOVA_CMDLINE'];",
      "if (!/cca/.test(cmdline)) {",
      "  var msg = 'ERROR: This is a CCA based project! Using 'cordova' rather than 'cca' will have unexpected results.' ;",
      "  console.error(msg);",
      "  process.exit(1);",
      "}"
      ];
  fs.writeFileSync(path, contents.join('\n'));
  fs.chmodSync(path, '777');
}
writeHook(path.join('hooks', 'before_prepare', 'cca-check.js'));
writeHook(path.join('hooks', 'before_platform_add', 'cca-check.js'));
...
```

#### <a name="apidoc.element.cca.utils.fatal"></a>[function <span class="apidocSignatureSpan">cca.utils.</span>fatal (msg)](#apidoc.element.cca.utils.fatal)
- description and source-code
```javascript
function fatal(msg) {
  console.error(msg);
  if (msg && msg.stack) console.error(msg.stack);
  exports.exit(1);
}
```
- example usage
```shell
...
  }

  // We only allow 'enable' and 'disable'; print an error if we were given something else.
  command = command.toLowerCase();
  if (command != 'enable' && command != 'disable') {
    var errorText = 'Invalid argument: ' + command + '. ';
    errorText += 'To enable or disable usage statistics collection, run ' + usage + '.';
    utils.fatal(errorText);
    return;
  }

  // Set analytics permission according to the given command.
  writePermission(command == 'enable');
  console.log('Usage statistics collection ' + command + 'd.');
}
...
```

#### <a name="apidoc.element.cca.utils.fixPathSlashes"></a>[function <span class="apidocSignatureSpan">cca.utils.</span>fixPathSlashes (p)](#apidoc.element.cca.utils.fixPathSlashes)
- description and source-code
```javascript
function fixPathSlashes(p) {
  return exports.isWindows() ? p.replace(/\//g, '\\') : p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cca.utils.isWindows"></a>[function <span class="apidocSignatureSpan">cca.utils.</span>isWindows ()](#apidoc.element.cca.utils.isWindows)
- description and source-code
```javascript
function isWindows() {
  return process.platform.slice(0, 3) == 'win';
}
```
- example usage
```shell
...
exports.fatal = function fatal(msg) {
console.error(msg);
if (msg && msg.stack) console.error(msg.stack);
exports.exit(1);
};

exports.fixPathSlashes = function fixPathSlashes(p) {
return exports.isWindows() ? p.replace(/\//g, '\\') : p;
};

exports.colorizeConsole = function colorizeConsole() {
var origWarn = console.warn;
console.warn = function() {
  var msg = [].slice.call(arguments).join(' ');
  origWarn.call(console, '\x1B[33m' + msg + '\x1B[39m');
...
```

#### <a name="apidoc.element.cca.utils.waitForKey"></a>[function <span class="apidocSignatureSpan">cca.utils.</span>waitForKey (opt_prompt)](#apidoc.element.cca.utils.waitForKey)
- description and source-code
```javascript
function waitForKey(opt_prompt) {
  opt_prompt = opt_prompt || 'Press the Any Key';
  process.stdout.write(opt_prompt);
  process.stdin.resume();
  try {
    // This fails if the process is a spawned child (likely a node bug);
    process.stdin.setRawMode(true);
  } catch (e) {
  }
  process.stdin.setEncoding('utf8');
  var d = Q.defer();
  process.stdin.on('data', function cont(key) {
    if (key == '\u0003') {
      process.exit(2);
    }
    process.stdin.removeListener('data', cont);
    process.stdin.pause();
    process.stdout.write('\n');
    d.resolve(key);
  });
  return d.promise;
}
```
- example usage
```shell
...
if (userConfig && userConfig.analytics) {
  return Q(userConfig.analytics.isAllowed);
}

// We have no record of permission, so ask away.
var promptText = 'Would you like to help make make this tool better by automatically sending usage statistics and error reports
to Google?\n';
promptText += 'This information will be used in accordance with the Google Privacy Policy (http://www.google.com/policies/privacy
). [y/n] ';
return utils.waitForKey(promptText)
.then(function(key) {
  var permission = (key.toLowerCase() == 'y');

  // Write the response to the config file and return it.
  writePermission(permission);
  return permission;
});
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
