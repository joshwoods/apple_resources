

- AppKit
- NSApplication
-  occlusionState 

Instance Property

# occlusionState

The occlusion state of the app.

macOS 10.9+

``` source
@MainActor
var occlusionState: NSApplication.OcclusionState { get }
```

## Discussion

The value of this property reflects whether any part of the app’s windows are visible to the user. Use this information to disable expensive screen updates when your app is not visible.

## See Also

### Related Documentation

class let didChangeOcclusionStateNotification: NSNotification.Name

Posted when the app’s occlusion state changes.

### Getting the Occlusion State

struct OcclusionState

This constant indicates whether at least part of any window owned by this app is visible.

