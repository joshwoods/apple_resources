

- Model I/O
- MDLObject
-  boundingBox(atTime:) 

Instance Method

# boundingBox(atTime:)

Returns the minimum region entirely enclosing the object’s contents at the specified time sample.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func boundingBox(atTime time: TimeInterval) -> MDLAxisAlignedBoundingBox
```

## Parameters 

`time`  

A timestamp referring to timed information in the asset.

## Return Value

The asset’s bounding box as of the specified time sample.

## Discussion

Objects may or may not provide spatial content. Subclasses of MDLObject that include spatial content, such as the MDLMesh class, implement this method to return the axis-aligned minimal region that entirely encloses such content. Objects without spatial content return an empty bounding box—that is, a MDLAxisAlignedBoundingBox structure whose `minBounds` field is greater than its `maxBounds` field.

Calling this method on an object that contains other objects (that is, one whose children property is not `nil` and references a nonempty container) recursively computes the combined bounding box enclosing of the object’s children.

## See Also

### Working with Objects in Space

var transform: (any MDLTransformComponent)?

A component that manages this object’s spatial transform and its changes over time.

