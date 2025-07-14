

- PHASE
- PHASEAssetRegistry
-  registerGlobalMetaParameter(metaParameterDefinition:) 

Instance Method

# registerGlobalMetaParameter(metaParameterDefinition:)

Registers a global metaparameter with the asset registry.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func registerGlobalMetaParameter(metaParameterDefinition: PHASEMetaParameterDefinition) throws -> PHASEGlobalMetaParameterAsset
```

## Parameters 

`metaParameterDefinition`  

A single parameter that controls the value of multiple parameters.

## Return Value

A global metaparameter object. If an error occurs, the function returns `nil`.

## Discussion

Global metaparameters attach to any number of sound event assets. When an app adjusts a global metaparameter at runtime, the change propagates immediately to all the attached sound events.

Note

Although you register a global metaparameter definition (PHASEMetaParameterDefinition) with this function, you receive a global metaparameter instance (PHASEMetaParameter) when you access the parameter by its identifier using the globalMetaParameters dictionary.

## See Also

### Registering Global Metaparameters

var globalMetaParameters: [String : PHASEMetaParameter]

A dictionary of metaparameters that all sound event assets share.

