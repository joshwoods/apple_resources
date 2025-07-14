

- Media Player
- MPMediaLibrary
-  authorizationStatus() 

Type Method

# authorizationStatus()

Returns whether the app can access the user’s media library.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func authorizationStatus() -> MPMediaLibraryAuthorizationStatus
```

## Return Value

The status representing whether the app has access to the user’s media library.

## See Also

### Getting the default media library

class func requestAuthorization((MPMediaLibraryAuthorizationStatus) -> Void)

Displays a user interface so that the user can authorize whether your app may view the media library’s contents.

enum MPMediaLibraryAuthorizationStatus

The list of possible states for authorization to access to the user’s media library.

class func `default`() -> MPMediaLibrary

Returns an instance of the default media library.

