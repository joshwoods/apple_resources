

- UIKit
- UIApplication
-  supportsMultipleScenes 

Instance Property

# supportsMultipleScenes

A Boolean value that indicates whether the app may display multiple scenes simultaneously.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var supportsMultipleScenes: Bool { get }
```

## Discussion

UIKit sets this property to true when the system allows the app to display multiple scenes and the app’s `Info.plist` file includes the UIApplicationSupportsMultipleScenes key with a value of true. If either of those conditions isn’t true, the value of this property is false.

Use the connectedScenes property to determine whether multiple scenes are present.

## See Also

### Getting scene information

var connectedScenes: Set&lt;UIScene>

The app’s currently connected scenes.

var openSessions: Set&lt;UISceneSession>

The sessions whose scenes are either currently active or archived by the system.

