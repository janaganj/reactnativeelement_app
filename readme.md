

Ref URL:
https://expo.io/@monte9/react-native-elements-app

GITHUB original:
https://github.com/react-native-elements/react-native-elements-app

Fix for the issue:

Expo fails to start the project: error Invalid regular expression: /(.*\\__fixtures__ #1074



hashes on your project:

\node_modules\metro-config\src\defaults\blacklist.js

var sharedBlacklist = [
  /node_modules[/\\]react[/\\]dist[/\\].*/,
  /website\/node_modules\/.*/,
  /heapCapture\/bundle\.js/,
  /.*\/__tests__\/.*/
];
change to:

var sharedBlacklist = [
  /node_modules[\/\\]react[\/\\]dist[\/\\].*/,
  /website\/node_modules\/.*/,
  /heapCapture\/bundle\.js/,
  /.*\/__tests__\/.*/
];
