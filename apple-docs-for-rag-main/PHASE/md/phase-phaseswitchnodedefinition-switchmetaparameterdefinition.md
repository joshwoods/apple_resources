

- PHASE
- PHASESwitchNodeDefinition
-  switchMetaParameterDefinition 

Instance Property

# switchMetaParameterDefinition

The meta parameter that holds the name of the child node to invoke.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var switchMetaParameterDefinition: PHASEStringMetaParameterDefinition { get }
```

## Discussion

The framework sets the value of this property to the init(switchMetaParameterDefinition:) argument.

## See Also

### Managing Child Nodes

func addSubtree(PHASESoundEventNodeDefinition, switchValue: String)

Adds a child node with the given switch value.

