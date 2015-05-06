# Cordova/PhoneGap SQLitePlugin (fork for PouchDB compatibility)

The [SQLite Plugin](https://github.com/litehelpers/Cordova-sqlite-storage) (also known as SQLite Storage) has gone through many changes recently (around early 2015) that broke compatibility with PouchDB. This is a fork representing an older commit ([ad4bd32](https://github.com/litehelpers/Cordova-sqlite-storage/commit/ad4bd32b831fb0be084475ee561eba6392280883)) back when it was passing the PouchDB test suite on both Android 4.0+ and iOS 7+.

You should only use this plugin if you need more than 50MB of storage on iOS, or you need native access to the SQLite `mydatabase.db` files. Otherwise just use the built-in IndexedDB/WebSQL adapters for PouchDB. They're faster and more reliable.

Usage
---

```
cordova plugin add https://github.com/nolanlawson/sqlite-plugin-fork
```

TODO
---

Fix the SQLite Plugin itself and make this repo obsolete.