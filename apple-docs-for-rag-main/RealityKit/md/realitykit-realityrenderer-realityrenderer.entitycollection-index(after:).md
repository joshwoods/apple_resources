

- RealityKit
- RealityRenderer
- RealityRenderer.EntityCollection
-  index(after:) 

Instance Method

# index(after:)

Returns the position immediately after the given index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor
func index(after i: Int) -> Int
```

## Parameters 

`i`  

A valid index of the collection. `i` must be less than `endIndex`.

## Return Value

The index value immediately after `i`.

## Discussion

The successor of an index must be well defined. For an index `i` into a collection `c`, calling `c.index(after: i)` returns the same index every time.

