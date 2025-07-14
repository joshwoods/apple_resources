

- UIKit
- UIDragDropSession
-  allowsMoveOperation 

Instance Property

# allowsMoveOperation

A Boolean value that indicates whether the drag session permits moving drag items within the same app.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsMoveOperation: Bool { get }
```

**Required**

## Discussion

A move operation can be applied only within the same app. Drag items shared with another app are always copied.

The `allowsMoveOperation` value is determined by the return value of the source app’s drag interaction delegate’s dragInteraction(_:sessionAllowsMoveOperation:) method. If `allowsMoveOperation` is true, the source app’s drop interaction delegate’s dropInteraction(_:sessionDidUpdate:) method can return a drop proposal for a UIDropOperation.move operation.

## See Also

### Checking for drag and drop session restrictions

var isRestrictedToDraggingApplication: Bool

A Boolean value that indicates whether the drag session is confined to the app that started the drag activity.

**Required**

