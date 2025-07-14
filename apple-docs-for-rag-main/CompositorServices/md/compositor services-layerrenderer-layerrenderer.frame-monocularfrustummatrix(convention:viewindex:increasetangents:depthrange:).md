

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
-  monocularFrustumMatrix(convention:viewIndex:increaseTangents:depthRange:) 

Instance Method

# monocularFrustumMatrix(convention:viewIndex:increaseTangents:depthRange:)

visionOS 2.0+

``` source
func monocularFrustumMatrix(
    convention: AxisDirectionConvention = .rightUpBack,
    viewIndex: Int,
    increaseTangents: SIMD4,
    depthRange: SIMD2
) -> matrix_float4x4
```

