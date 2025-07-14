

- Media Player
- MPMediaLibrary
-  requestAuthorization(\_:) 

Type Method

# requestAuthorization(\_:)

Displays a user interface so that the user can authorize whether your app may view the media library’s contents.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func requestAuthorization(_ completionHandler: @escaping (MPMediaLibraryAuthorizationStatus) -> Void)
```

``` source
class func requestAuthorization() async -> MPMediaLibraryAuthorizationStatus
```

## Parameters 

`completionHandler`  

A block that the system calls after the user chooses whether to authorize the app.

status  
The status chosen by the user.

## See Also

### Getting the default media library

class func authorizationStatus() -> MPMediaLibraryAuthorizationStatus

Returns whether the app can access the user’s media library.

enum MPMediaLibraryAuthorizationStatus

The list of possible states for authorization to access to the user’s media library.

class func `default`() -> MPMediaLibrary

Returns an instance of the default media library.

