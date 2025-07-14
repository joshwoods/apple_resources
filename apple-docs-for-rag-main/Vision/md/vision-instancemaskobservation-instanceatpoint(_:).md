

- Vision
- InstanceMaskObservation
-  instanceAtPoint(\_:) 

Instance Method

# instanceAtPoint(\_:)

Returns an instance at the point you specify.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func instanceAtPoint(_ point: NormalizedPoint) -> IndexSet
```

## See Also

### Getting instances

let allInstances: IndexSet

The collection that contains all instances, excluding the background.

let allInstancesMask: PixelBufferObservation

The resulting mask that represents all instances.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

