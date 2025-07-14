

- Vision
- InstanceMaskObservation
-  allInstancesMask 

Instance Property

# allInstancesMask

The resulting mask that represents all instances.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let allInstancesMask: PixelBufferObservation
```

## Discussion

A pixel can only correspond to one instance. A `0` represents the background, and all other values represent the indices of the instances.

## See Also

### Getting instances

func instanceAtPoint(NormalizedPoint) -> IndexSet

Returns an instance at the point you specify.

let allInstances: IndexSet

The collection that contains all instances, excluding the background.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

