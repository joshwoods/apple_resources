

- Media Player
-  MPMediaLibraryAuthorizationStatus 

Enumeration

# MPMediaLibraryAuthorizationStatus

The list of possible states for authorization to access to the user’s media library.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum MPMediaLibraryAuthorizationStatus
```

## Topics

### Authorization statuses

case notDetermined

The user hasn’t determined whether to authorize the use of their media library.

case denied

The app may not access the items in the user’s media library.

case restricted

The app may access some of the content in the user’s media library.

case authorized

Your app may access items in the user’s media library.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the default media library

class func requestAuthorization((MPMediaLibraryAuthorizationStatus) -> Void)

Displays a user interface so that the user can authorize whether your app may view the media library’s contents.

class func authorizationStatus() -> MPMediaLibraryAuthorizationStatus

Returns whether the app can access the user’s media library.

class func `default`() -> MPMediaLibrary

Returns an instance of the default media library.

