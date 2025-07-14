

- PHASE
- PHASENumberMetaParameterDefinition
-  init(value:identifier:) 

Initializer

# init(value:identifier:)

Creates a specification for a named metaparameter with the given numeric value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    value: Double,
    identifier: String
)
```

## Parameters 

`value`  

A default value for the metaparameter specification.

`identifier`  

A unique name for the metaparameter specification.

## See Also

### Creating a Metaparameter Definition

convenience init(value: Double)

Creates a specification for a metaparameter with the given numeric value.

init(value: Double, minimum: Double, maximum: Double)

Creates a specification for a metaparameter with the given numeric value and range.

convenience init(value: Double, minimum: Double, maximum: Double, identifier: String)

Creates a specification for a named metaparameter with the given numeric value and range.

