

- PHASE
- PHASEMappedMetaParameterDefinition
-  init(inputMetaParameterDefinition:envelope:) 

Initializer

# init(inputMetaParameterDefinition:envelope:)

Creates a specification for a metaparameter that the app plots on a graph defined by the given set of curves.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    inputMetaParameterDefinition: PHASENumberMetaParameterDefinition,
    envelope: PHASEEnvelope
)
```

## Parameters 

`inputMetaParameterDefinition`  

A metaparameter that contains an input value.

`envelope`  

A set of curves that graph the input value.

## See Also

### Creating a Mapped Metaparameter

convenience init(inputMetaParameterDefinition: PHASENumberMetaParameterDefinition, envelope: PHASEEnvelope, identifier: String)

Creates a specification for a named metaparameter that the app plots on a graph defined by the given set of curves.

