

- RealityKit
- ShapeResource
-  offsetBy(rotation:translation:) 

Instance Method

# offsetBy(rotation:translation:)

Creates a new shape resource by applying a rotation and a translation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func offsetBy(
    rotation: simd_quatf = simd_quatf(ix: 0, iy: 0, iz: 0, r: 1),
    translation: SIMD3 = SIMD3()
) -> ShapeResource
```

## Parameters 

`rotation`  

The rotation to apply to the existing shape resource.

`translation`  

The translation to apply to the existing shape resource.

## Return Value

The transformed resource.

## See Also

### Transforming a shape

func offsetBy(rotation: simd_quatf) -> ShapeResource

Creates a new shape resource by applying a rotation.

func offsetBy(translation: SIMD3&lt;Float>) -> ShapeResource

Creates a new shape resource by applying a translation.

