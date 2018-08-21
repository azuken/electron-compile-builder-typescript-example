# Electron Compile with Typescript + SASS that makes a working installer using electron-builder


Dev
```
yarn start
```

Build to a folder
```
yarn run pre-pack
yarn run pack
```

Build to an installer
```
yarn dist
```


## Notes
Only tested on windows.

The package.json has:
```
  "build": {
    "electronCompile": false
  }
```
We do this build step manually.
Looks like electon-builder is messing up something when it tries to do the electron compile step.

You probably need to remove the `.cache` dir at some stage.