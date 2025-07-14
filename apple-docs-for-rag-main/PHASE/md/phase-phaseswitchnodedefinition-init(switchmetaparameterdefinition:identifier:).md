

- PHASE
- PHASESwitchNodeDefinition
-  init(switchMetaParameterDefinition:identifier:) 

Initializer

# init(switchMetaParameterDefinition:identifier:)

Creates a named node that invokes a child node based on the value of the given parameter.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    switchMetaParameterDefinition: PHASEStringMetaParameterDefinition,
    identifier: String
)
```

## Parameters 

`switchMetaParameterDefinition`  

A string meta parameter that specifies the child node identifier to pass invocation on to.

`identifier`  

A unique name for the switch node.

## See Also

### Creating a Node

init(switchMetaParameterDefinition: PHASEStringMetaParameterDefinition)

Creates a node that invokes a child node based on the value of the given parameter.

