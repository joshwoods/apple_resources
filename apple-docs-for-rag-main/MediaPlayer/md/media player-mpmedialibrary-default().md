

- Media Player
- MPMediaLibrary
-  default() 

Type Method

# default()

Returns an instance of the default media library.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func `default`() -> MPMediaLibrary
```

## Return Value

The user’s default media library.

## See Also

### Getting the default media library

class func requestAuthorization((MPMediaLibraryAuthorizationStatus) -> Void)

Displays a user interface so that the user can authorize whether your app may view the media library’s contents.

class func authorizationStatus() -> MPMediaLibraryAuthorizationStatus

Returns whether the app can access the user’s media library.

enum MPMediaLibraryAuthorizationStatus

The list of possible states for authorization to access to the user’s media library.

