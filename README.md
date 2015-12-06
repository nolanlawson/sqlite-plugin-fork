# Cordova/PhoneGap SQLitePlugin fork ![project unmaintained](https://img.shields.io/badge/project-unmaintained-red.svg)

This is a snapshot of the [SQLite Plugin](https://github.com/litehelpers/Cordova-sqlite-storage) back when it was passing the PouchDB test suite on Android/iOS at 100%. Since then, it has regressed.

## Deprecation notice

Instead of this repo, you can also use the `androidDatabaseImplementation` option instead: http://pouchdb.com/api.html#create_database . Set it to `2` if you want the older implementation, which has better compatibility with PouchDB.

Or better yet, just don't use the SQLite Plugin on Android. It's slower, less stable, and doesn't offer any higher storage limit than regular WebSQL/IndexedDB: http://pouchdb.com/faq.html#data_limits

Original SQLite PLugin documentation follows.

## Original documentation

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
