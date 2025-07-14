

- RealityKit
- SkeletalPosesComponent
-  init(poses:) 

Initializer

# init(poses:)

Creates a component value with the provided poses.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(poses: [SkeletalPose])
```

## Parameters 

`poses`  

The pose values, arranged in any order of your choosing.

## Discussion

Warning

When multiple poses share the same identifier, only the first one is accessible using its identifier.

