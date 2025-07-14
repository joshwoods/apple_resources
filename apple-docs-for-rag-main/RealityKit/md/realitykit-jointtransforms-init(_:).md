

- RealityKit
- JointTransforms
-  init(\_:) 

Initializer

# init(\_:)

Initializes a collection of transforms of a specific type for a single skeletal pose.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(_ transforms: S) where S : Sequence, S.Element == Transform
```

## Parameters 

`transforms`  

An array of position, rotation, and scale data for the joints.

## See Also

### Creating joint transforms

init()

Initializes a collection of animatable transforms for a single skeletal pose.

init(arrayLiteral: Transform...)

Initializes a collection of animatable transforms using the argument elements for a single skeletal pose.

