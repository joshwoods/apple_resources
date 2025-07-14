

- PHASE
- PHASEAssetRegistry
-  globalMetaParameters 

Instance Property

# globalMetaParameters

A dictionary of metaparameters that all sound event assets share.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var globalMetaParameters: [String : PHASEMetaParameter] { get }
```

## Discussion

When you change a value for a metaparameter in this dictionary, every sound event attached to the metaparameter observes the change. The dictionary key is the identifier of the PHASEMetaParameterDefinition you pass into registerGlobalMetaParameter(metaParameterDefinition:).

Tip

To adjust a value for a single sound event, access the metaparameter through the metaParameters property instead.

## See Also

### Registering Global Metaparameters

func registerGlobalMetaParameter(metaParameterDefinition: PHASEMetaParameterDefinition) throws -> PHASEGlobalMetaParameterAsset

Registers a global metaparameter with the asset registry.

