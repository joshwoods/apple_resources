

- Game Controller
- GCController
-  isSnapshot 

Instance Property

# isSnapshot

A Boolean value that indicates whether the controller is a snapshot of a controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var isSnapshot: Bool { get }
```

## Discussion

If true, the controller is a snapshot of a controller. A snapshot is a copy of a real or virtual controller at a moment in time with its current element values. If false, the controller is a real or virtual controller.

## See Also

### Creating snapshots

class func withExtendedGamepad() -> GCController

Returns a snapshot of a newly created controller with an extended gamepad profile.

class func withMicroGamepad() -> GCController

Returns a snapshot of a newly created controller with a micro gamepad profile.

func capture() -> GCController

Returns a snapshot of the controller with its current element values.

