

- SwiftUI
- RotateGesture
-  init(minimumAngleDelta:) 

Initializer

# init(minimumAngleDelta:)

Creates a rotation gesture with a minimum delta for the gesture to start.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
init(minimumAngleDelta: Angle = .degrees(1))
```

## Parameters 

`minimumAngleDelta`  

The minimum delta required before the gesture starts. The default value is a one-degree angle.

## See Also

### Creating the gesture

var minimumAngleDelta: Angle

The minimum delta required before the gesture succeeds.

