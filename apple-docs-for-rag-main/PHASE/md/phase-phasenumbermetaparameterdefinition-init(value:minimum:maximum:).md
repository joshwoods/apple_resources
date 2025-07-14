

- PHASE
- PHASENumberMetaParameterDefinition
-  init(value:minimum:maximum:) 

Initializer

# init(value:minimum:maximum:)

Creates a specification for a metaparameter with the given numeric value and range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    value: Double,
    minimum: Double,
    maximum: Double
)
```

## Parameters 

`value`  

A default value for the metaparameter specification.

`minimum`  

The lowest possible number for the value.

`maximum`  

The highest possible number for the value.

## See Also

### Creating a Metaparameter Definition

convenience init(value: Double)

Creates a specification for a metaparameter with the given numeric value.

convenience init(value: Double, identifier: String)

Creates a specification for a named metaparameter with the given numeric value.

convenience init(value: Double, minimum: Double, maximum: Double, identifier: String)

Creates a specification for a named metaparameter with the given numeric value and range.

