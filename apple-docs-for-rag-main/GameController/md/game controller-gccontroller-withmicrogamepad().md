

- Game Controller
- GCController
-  withMicroGamepad() 

Type Method

# withMicroGamepad()

Returns a snapshot of a newly created controller with a micro gamepad profile.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func withMicroGamepad() -> GCController
```

## Return Value

A snapshot with a micro gamepad profile.

## Discussion

A snapshot is a copy of a real or virtual controller at a moment in time with its current element values. Unlike other controllers, you can set the values of a snapshot’s GCControllerElement objects.

## See Also

### Creating snapshots

class func withExtendedGamepad() -> GCController

Returns a snapshot of a newly created controller with an extended gamepad profile.

func capture() -> GCController

Returns a snapshot of the controller with its current element values.

var isSnapshot: Bool

A Boolean value that indicates whether the controller is a snapshot of a controller.

