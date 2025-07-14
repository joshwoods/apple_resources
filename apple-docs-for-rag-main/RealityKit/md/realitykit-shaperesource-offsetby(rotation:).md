

- RealityKit
- ShapeResource
-  offsetBy(rotation:) 

Instance Method

# offsetBy(rotation:)

Creates a new shape resource by applying a rotation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func offsetBy(rotation: simd_quatf) -> ShapeResource
```

## Parameters 

`rotation`  

The rotation to apply to the existing shape resource.

## Return Value

The transformed resource.

## See Also

### Transforming a shape

func offsetBy(translation: SIMD3&lt;Float>) -> ShapeResource

Creates a new shape resource by applying a translation.

func offsetBy(rotation: simd_quatf, translation: SIMD3&lt;Float>) -> ShapeResource

Creates a new shape resource by applying a rotation and a translation.

