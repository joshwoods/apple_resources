

- Media Player
-  MPMediaLibrary 

Class

# MPMediaLibrary

An object that represents the state of synced media items on a device.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMediaLibrary
```

## Overview

A user may sync their device, changing the contents on the device, while your app is running. You can use the notification provided by this class to ensure that your app’s cache of the user’s library is up-to-date.

To retrieve media items from the media library, build a custom query as described in MPMediaPropertyPredicate and MPMediaQuery.

## Topics

### Getting the default media library

class func requestAuthorization((MPMediaLibraryAuthorizationStatus) -> Void)

Displays a user interface so that the user can authorize whether your app may view the media library’s contents.

class func authorizationStatus() -> MPMediaLibraryAuthorizationStatus

Returns whether the app can access the user’s media library.

enum MPMediaLibraryAuthorizationStatus

The list of possible states for authorization to access to the user’s media library.

class func `default`() -> MPMediaLibrary

Returns an instance of the default media library.

### Receiving notifications when the user’s library changes

func beginGeneratingLibraryChangeNotifications()

Asks the media library to turn on notifications for whenever the library changes.

func endGeneratingLibraryChangeNotifications()

Asks the media library to turn off notifications for whenever the library changes.

var lastModifiedDate: Date

The calendar date on which the media library was last modified.

### Retrieving a playlist from the media library

func getPlaylist(with: UUID, creationMetadata: MPMediaPlaylistCreationMetadata?, completionHandler: (MPMediaPlaylist?, (any Error)?) -> Void)

Retrieves an app maintained existing playlist or creates a new playlist when no playlist exists.

### Adding an item to the media library

func addItem(withProductID: String, completionHandler: (([MPMediaEntity], (any Error)?) -> Void)?)

Adds the designated item to the user’s music library.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

