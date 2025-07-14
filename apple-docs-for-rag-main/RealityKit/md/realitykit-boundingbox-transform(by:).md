

- RealityKit
- BoundingBox
-  transform(by:) 

Instance Method

# transform(by:)

Transforms the bounding box.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
mutating func transform(by transform: float4x4)
```

## Parameters 

`transform`  

The transform to apply to the box.

## See Also

### Transforming a bounding box

func transformed(by: float4x4) -> BoundingBox

Transforms the bounding box and finds the bounds of the result.

