

- RealityKit
- GeometricPin
-  init(named:offsetPosition:offsetOrientation:) 

Initializer

# init(named:offsetPosition:offsetOrientation:)

Creates a geometric pin that identifies a local position and orientation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    named name: String,
    offsetPosition: SIMD3 = SIMD3(0, 0, 0),
    offsetOrientation: simd_quatf = simd_quatf(ix: 0, iy: 0, iz: 0, r: 1)
)
```

## Parameters 

`name`  

Name of the `GeometricPin` in the namespace of the owning entity.

`offsetPosition`  

Adjustment of the `GeometricPin` position in the local coordinate frame.

`offsetOrientation`  

Adjustment of the `GeometricPin` orientation in the local coordinate frame.

