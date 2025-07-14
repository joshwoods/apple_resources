

- PHASE
- PHASESwitchNodeDefinition
-  addSubtree(\_:switchValue:) 

Instance Method

# addSubtree(\_:switchValue:)

Adds a child node with the given switch value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func addSubtree(
    _ subtree: PHASESoundEventNodeDefinition,
    switchValue: String
)
```

## Parameters 

`subtree`  

The child node, which itself can contain a hierarchical tree of descendent nodes.

`switchValue`  

The meta parameter value that invokes the `subtree` child node.

## See Also

### Managing Child Nodes

var switchMetaParameterDefinition: PHASEStringMetaParameterDefinition

The meta parameter that holds the name of the child node to invoke.

