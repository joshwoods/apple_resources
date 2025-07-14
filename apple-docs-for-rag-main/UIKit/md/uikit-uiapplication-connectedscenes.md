

- UIKit
- UIApplication
-  connectedScenes 

Instance Property

# connectedScenes

The app’s currently connected scenes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var connectedScenes: Set { get }
```

## Discussion

Connected scenes are those that are in memory and potentially doing active work. A connected scene may be in the foreground or background, and it may be onscreen or offscreen.

## See Also

### Getting scene information

var supportsMultipleScenes: Bool

A Boolean value that indicates whether the app may display multiple scenes simultaneously.

var openSessions: Set&lt;UISceneSession>

The sessions whose scenes are either currently active or archived by the system.

