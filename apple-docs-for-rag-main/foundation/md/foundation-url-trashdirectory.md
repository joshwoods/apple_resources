

- Foundation
- URL
-  trashDirectory 

Type Property

# trashDirectory

The standard trash directory.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
static var trashDirectory: URL { get }
```

## Discussion

In iOS, this directory is within the app’s sandbox directory. In macOS, it’s within the app’s sandbox directory for sandboxed apps, or in the current user’s home directory `(~/.Trash)` if the app isn’t sandboxed.

This computed property is equivalent to calling NSSearchPathForDirectoriesInDomains(_:_:_:) with the FileManager.SearchPathDirectory.trashDirectory parameter.

## See Also

### Accessing common directories

static var applicationDirectory: URL

The standard directory for apps.

static var applicationSupportDirectory: URL

The standard directory for application support files.

static var cachesDirectory: URL

The standard directory for discardable cache files.

static var desktopDirectory: URL

The standard directory for files on the desktop.

static var documentsDirectory: URL

The standard directory for document files.

static var downloadsDirectory: URL

The standard directory for download files.

static var libraryDirectory: URL

The standard directory for documentation, support, and configuration files.

static var moviesDirectory: URL

The standard directory for movie files.

static var musicDirectory: URL

The standard directory for music files.

static var picturesDirectory: URL

The standard directory for image files.

static var sharedPublicDirectory: URL

The standard directory for publicly shared files.

static var temporaryDirectory: URL

The standard directory for temporary files.

static var userDirectory: URL

The container directory of user home directories.

