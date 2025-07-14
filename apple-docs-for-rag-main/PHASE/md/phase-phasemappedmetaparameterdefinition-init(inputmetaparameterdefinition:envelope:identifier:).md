

- PHASE
- PHASEMappedMetaParameterDefinition
-  init(inputMetaParameterDefinition:envelope:identifier:) 

Initializer

# init(inputMetaParameterDefinition:envelope:identifier:)

Creates a specification for a named metaparameter that the app plots on a graph defined by the given set of curves.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    inputMetaParameterDefinition: PHASENumberMetaParameterDefinition,
    envelope: PHASEEnvelope,
    identifier: String
)
```

## Parameters 

`inputMetaParameterDefinition`  

A metaparameter that contains an input value.

`envelope`  

A set of curves that graph the input value.

`identifier`  

A unique name for the metaparameter specification.

## See Also

### Creating a Mapped Metaparameter

init(inputMetaParameterDefinition: PHASENumberMetaParameterDefinition, envelope: PHASEEnvelope)

Creates a specification for a metaparameter that the app plots on a graph defined by the given set of curves.

