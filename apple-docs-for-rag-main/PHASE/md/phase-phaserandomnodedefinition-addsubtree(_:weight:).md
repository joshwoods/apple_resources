

- PHASE
- PHASERandomNodeDefinition
-  addSubtree(\_:weight:) 

Instance Method

# addSubtree(\_:weight:)

Adds a node tree that’s one of the random-selection options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func addSubtree(
    _ subtree: PHASESoundEventNodeDefinition,
    weight: NSNumber
)
```

## Parameters 

`subtree`  

The child node, which itself can contain a hierarchical tree of descendent nodes.

`weight`  

A number that implements favoritism in the random selection.

