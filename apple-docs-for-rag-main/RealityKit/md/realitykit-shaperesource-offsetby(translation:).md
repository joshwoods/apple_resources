

- RealityKit
- ShapeResource
-  offsetBy(translation:) 

Instance Method

# offsetBy(translation:)

Creates a new shape resource by applying a translation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func offsetBy(translation: SIMD3) -> ShapeResource
```

## Parameters 

`translation`  

The translation to apply to the existing shape resource.

## Return Value

The transformed resource.

## See Also

### Transforming a shape

func offsetBy(rotation: simd_quatf) -> ShapeResource

Creates a new shape resource by applying a rotation.

func offsetBy(rotation: simd_quatf, translation: SIMD3&lt;Float>) -> ShapeResource

Creates a new shape resource by applying a rotation and a translation.

