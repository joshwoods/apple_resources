

- Game Controller
- GCController
-  current 

Type Property

# current

The most recently used game controller.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class var current: GCController? { get }
```

## Discussion

Use this property for a single-player game when you don’t need to distinguish the input from multiple controllers simultaneously.

## See Also

### Handling multiple controllers

static let GCControllerDidBecomeCurrent: NSNotification.Name

A notification that posts when a controller becomes the current controller.

static let GCControllerDidStopBeingCurrent: NSNotification.Name

A notification that posts when a controller stops being the current controller.

