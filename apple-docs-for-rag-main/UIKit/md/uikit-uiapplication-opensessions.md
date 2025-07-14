

- UIKit
- UIApplication
-  openSessions 

Instance Property

# openSessions

The sessions whose scenes are either currently active or archived by the system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var openSessions: Set { get }
```

## Discussion

An archived session doesn’t have a connected scene, but a snapshot of its UI does appear in the app switcher. When the user selects that UI in the app switcher, the system asks your app to recreate the UI from the session information.

## See Also

### Getting scene information

var supportsMultipleScenes: Bool

A Boolean value that indicates whether the app may display multiple scenes simultaneously.

var connectedScenes: Set&lt;UIScene>

The app’s currently connected scenes.

