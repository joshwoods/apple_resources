

- iTunes Library
-  ITLibrary 

Class

# ITLibrary

This class serves as the entry point to the iTunesLibrary framework.

Mac Catalyst 14.0+macOS 10.13+

``` source
class ITLibrary
```

## Overview

Use the ITLibrary properties and methods to retrieve media items (tracks) and playlists from the user’s iTunes library. ITLibrary also provides methods for extracting artwork from a media file that may or may not be in the iTunes library. Sandboxed and nonsandboxed apps can also use iTunes’ ability to extract artwork.

Important

A person needs to grant your app permission before it can access their iTunes library. Add the NSAppleMusicUsageDescription key to your app’s `Info.plist` file, and include a description of how you intend to use their library. If this key isn’t present, the system terminates your app when it tries to access the library.

## Topics

### Essentials

convenience init(apiVersion: String) throws

Initializes an instance of ITLibrary that can retrieve media entities.

init(apiVersion: String, options: ITLibInitOptions) throws

Initializes an instance of `ITLibrary` that can retrieve media entities.

enum ITLibInitOptions

These constants describe initialization options for an iTunes library.

### Getting iTunes Library Info

var allMediaItems: [ITLibMediaItem]

All the media items (tracks) in the iTunes library.

var allPlaylists: [ITLibPlaylist]

All the playlists in the iTunes library.

var apiMajorVersion: Int

The major version number of the API the iTunesLibrary framework exposes.

var apiMinorVersion: Int

The minor version number of the API the iTunesLibrary framework exposes.

var applicationVersion: String

The version of iTunes that created or modified the iTunes library you’re accessing.

var mediaFolderLocation: URL?

The location of the iTunes music folder.

var shouldShowContentRating: Bool

A Boolean value indicating whether to show content rating labels.

### Loading and Unloading Data

func reloadData() -> Bool

Refreshes the data that the framework uses.

func unloadData()

Unloads the data that the framework uses.

### Accessing Artwork

func artwork(forMediaFile: URL) -> ITLibArtwork?

Retrieves the artwork from a media file that may or may not be in the iTunes library.

### Deprecated

var features: ITLibExportFeature

A bitwise OR combination of the features of this library.

Deprecated

enum ITLibExportFeature

These constants describe the features that an iTunes library supports.

var musicFolderLocation: URL?

The location of the iTunes music folder.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

