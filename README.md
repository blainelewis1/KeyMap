# KeyMap

This repository contains the source for Chrome Extension that visualises keyboard shortcuts on a keyboard to improve their memorability.

The Chrome extension can be found at https://chrome.google.com/webstore/detail/keymap/fpminkfnndfokkmoobbngdpnijbcajkl

The repository also contains the source code for an npm package that allows others to use KeyMap in their applications.

More details on KeyMap can be found at blainelewis1.ca/KeyMap

# Developing

Developing the npm packge is a bit tricky, the Chrome extension needs React as a devDependency, but the npm package can't be bundled with React or it breaks.

If developing the Chrome extension add this line to `package.json`:

```
  "devDependencies": {
    "react": "^16.13.1",
    "react-dom": "^16.13.1"
  },
```

At some point the right thing to do is to put the extension in it's own repository and then have it import KeyMap as a dependency but that makes too much sense.
