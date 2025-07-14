

- SceneKit
- SCNPhysicsShape
-  init(shapes:transforms:) 

Initializer

# init(shapes:transforms:)

Creates a new physics shape by combining others.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    shapes: [SCNPhysicsShape],
    transforms: [NSValue]?
)
```

## Parameters 

`shapes`  

An array of SCNPhysicsShape objects.

`transforms`  

An array of NSValue objects containing SCNMatrix4 values, each of which is a transform for the physics shape at the corresponding index in the `shapes` parameter.

## Return Value

A new physics shape object.

## Discussion

An individual physics shape is defined in its own local coordinate space. Therefore, to describe the positions and orientations of multiple shapes relative to one another, you must use coordinate transformations.

