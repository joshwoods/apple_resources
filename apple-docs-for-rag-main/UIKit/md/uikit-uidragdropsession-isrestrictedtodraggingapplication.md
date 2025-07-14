

- UIKit
- UIDragDropSession
-  isRestrictedToDraggingApplication 

Instance Property

# isRestrictedToDraggingApplication

A Boolean value that indicates whether the drag session is confined to the app that started the drag activity.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isRestrictedToDraggingApplication: Bool { get }
```

**Required**

## Discussion

The value for this property is set by the source app’s drag interaction delegate method dragInteraction(_:sessionIsRestrictedToDraggingApplication:). If the value is true, the drag session is restricted to the app that started the drag operation.

## See Also

### Checking for drag and drop session restrictions

var allowsMoveOperation: Bool

A Boolean value that indicates whether the drag session permits moving drag items within the same app.

**Required**

