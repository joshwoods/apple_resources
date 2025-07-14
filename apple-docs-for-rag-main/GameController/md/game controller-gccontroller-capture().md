

- Game Controller
- GCController
-  capture() 

Instance Method

# capture()

Returns a snapshot of the controller with its current element values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func capture() -> GCController
```

## Return Value

A snapshot of the controller.

## Discussion

A snapshot is a copy of a real or virtual controller at a moment in time with its current element values. Unlike other controllers, you can set the values of a snapshot’s GCControllerElement objects.

## See Also

### Creating snapshots

class func withExtendedGamepad() -> GCController

Returns a snapshot of a newly created controller with an extended gamepad profile.

class func withMicroGamepad() -> GCController

Returns a snapshot of a newly created controller with a micro gamepad profile.

var isSnapshot: Bool

A Boolean value that indicates whether the controller is a snapshot of a controller.

