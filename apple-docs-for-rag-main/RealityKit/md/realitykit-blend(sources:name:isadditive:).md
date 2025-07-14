

- RealityKit
-  blend(sources:name:isAdditive:) 

Function

# blend(sources:name:isAdditive:)

Combines the animations that result from the individual blend-tree nodes of the given array to a single blend-tree node.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
func blend(
    sources: [any BlendTreeNode],
    name: String = "",
    isAdditive: Bool = false
) -> any BlendTreeNode
```

## Parameters 

`sources`  

The blend-tree nodes to combine.

`name`  

A unique name for the combined node.

`isAdditive`  

A Boolean value that indicates whether the animation builds on the current state of the target entity, or resets the state before running.

## Return Value

A blend-tree node that combines the given animations.

## See Also

### Blending animations

func blend(any BlendTreeNode, any BlendTreeNode, name: String, isAdditive: Bool) -> any BlendTreeNode

Combines the animations that result from two blend-tree nodes into a single blend-tree node.

