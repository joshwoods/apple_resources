

- UIKit
- UIPasteboard
-  changeCount 

Instance Property

# changeCount

The number of times the pasteboard’s contents change.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var changeCount: Int { get }
```

## Discussion

Whenever the contents of a pasteboard changes—specifically, when pasteboard items are added, modified, or removed—`UIPasteboard` increments the value of this property. After it increments the change count, UIPasteboard posts the notifications named changedNotification (for additions and modifications) and removedNotification (for removals). These notifications include (in the `userInfo` dictionary) the types of the pasteboard items added or removed. Because `UIPasteboard` waits until the end of the current event loop before incrementing the change count, notifications can be batched. The class also updates the change count when an app reactivates and another app has changed the pasteboard contents. When users restart a device, the change count is reset to zero.

## See Also

### Getting and setting pasteboard attributes

var name: UIPasteboard.Name

The name of the pasteboard.

