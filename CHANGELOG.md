## 2.1.0

* Updated native build scripts
* Bumped min Flutter version to 3.10.0

## 2.0.0

* Added Windows platform support using BITS ([Background Intelligent Transfer Service](https://learn.microsoft.com/en-us/windows/win32/bits/background-intelligent-transfer-service-portal))

### BREAKING CHANGES
* All `downloadId`s parameters and returns are now `dynamic` as mobile platforms returns ids as integers and Windows returns a GUID String. This may or may not break some apps logic.

## 1.2.0

* Added error messaging returning on `DownloadStatus.failed` and reason on `DownloadStatus.paused`
* Added log messages on native side
* Added a function to reattach the download progress stream to a download on Android

## 1.1.1

* Fixed `fileNotFoundException` on `openFile()` in Android 10
* Fixed download progress stops updating after 15 seconds

## 1.1.0

* Updated Dart to 2.18 and Flutter 3.3
* Renamed `Progress` class to `DownloadProgress` to avoid collision with other classes or plugins
* Added a explicit documentation related to return of download()
* Added a method to request Storage Access permition on Android 9 or bellow
* Fixed download on urls that have invalid filename chars

## 1.0.3

* Fixed Android `divideByZero` exception

## 1.0.2

* Fixed iOS download with empty filename

## 1.0.1

* Added documentation comments on public API

## 1.0.0

* Initial version with Android and iOS support
