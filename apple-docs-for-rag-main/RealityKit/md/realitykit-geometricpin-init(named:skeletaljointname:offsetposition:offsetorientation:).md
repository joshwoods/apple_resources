

- RealityKit
- GeometricPin
-  init(named:skeletalJointName:offsetPosition:offsetOrientation:) 

Initializer

# init(named:skeletalJointName:offsetPosition:offsetOrientation:)

Creates a geometric pin that attaches to a skeletal joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    named name: String,
    skeletalJointName: String,
    offsetPosition: SIMD3 = SIMD3(0, 0, 0),
    offsetOrientation: simd_quatf = simd_quatf(ix: 0, iy: 0, iz: 0, r: 1)
)
```

## Parameters 

`name`  

Name of the `GeometricPin` in the namespace of the owning entity.

`skeletalJointName`  

Name of the skeletal joint that this pin attaches to.

`offsetPosition`  

Adjustment of the `GeometricPin` position in the coordinate frame of the joint.

`offsetOrientation`  

Adjustment of the `GeometricPin` orientation in the coordinate frame of the joint.

## Discussion

The current animated joint transform defines the position and orientation of the pin.

