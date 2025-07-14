

- RealityKit
- BlendShapeWeightsSet
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accessor for reading a blend shape weights data in the set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
subscript(blendShapeName: String) -> BlendShapeWeightsSet.Element? { get }
```

## Parameters 

`blendShapeName`  

The name of the blend shape to be returned.

## Return Value

Blend shape weights data associated with the given name owned by this set, or nil if not found.

