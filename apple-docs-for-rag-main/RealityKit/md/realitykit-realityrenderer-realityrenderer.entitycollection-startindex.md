

- RealityKit
- RealityRenderer
- RealityRenderer.EntityCollection
-  startIndex 

Instance Property

# startIndex

The position of the first element in a nonempty collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor
var startIndex: Int { get }
```

## Discussion

If the collection is empty, `startIndex` is equal to `endIndex`.

