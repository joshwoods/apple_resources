

- RealityKit
- Entity
-  anchor 

Instance Property

# anchor

The nearest ancestor entity that can act as an anchor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var anchor: (any HasAnchoring)? { get }
```

## Discussion

This property returns `nil` if no ancestor can act as an anchor. An entity can act as an anchor if it adopts the HasAnchoring protocol. Just because an ancestor can be anchored doesn’t mean that it is. Inspect the isAnchored property to see if an entity (or one of its ancestors) is anchored.

