

- RealityKit
- ModelSortGroup
-  planarUIPlacement 

Instance Property

# planarUIPlacement

A planar placement instance that controls how the renderer draws a model relative to a planar mesh or a SwiftUI view that’s coplanar and overlapping.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var planarUIPlacement: ModelSortGroup.PlanarUIPlacement? { get }
```

## Discussion

Set to `nil` when the renderer doesn’t need planar sort the group. setting the property to `nil`.

