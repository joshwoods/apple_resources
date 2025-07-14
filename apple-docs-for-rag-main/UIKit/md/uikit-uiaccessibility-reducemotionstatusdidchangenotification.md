

- UIKit
- UIAccessibility
-  reduceMotionStatusDidChangeNotification 

Type Property

# reduceMotionStatusDidChangeNotification

A notification that UIKit posts when the system’s Reduce Motion setting changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let reduceMotionStatusDidChangeNotification: NSNotification.Name
```

## Discussion

This notification doesn’t include a parameter. Observe this notification using the default notification center.

## See Also

### Motion

static let shakeToUndoDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Shake to Undo setting changes.

