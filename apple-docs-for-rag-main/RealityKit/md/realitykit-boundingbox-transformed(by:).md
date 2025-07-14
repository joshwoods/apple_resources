

- RealityKit
- BoundingBox
-  transformed(by:) 

Instance Method

# transformed(by:)

Transforms the bounding box and finds the bounds of the result.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
func transformed(by transform: float4x4) -> BoundingBox
```

## Parameters 

`transform`  

The transform to apply to the box.

## Return Value

The bounds of the transformed box.

## See Also

### Transforming a bounding box

func transform(by: float4x4)

Transforms the bounding box.

