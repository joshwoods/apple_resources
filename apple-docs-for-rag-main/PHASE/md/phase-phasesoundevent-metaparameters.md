

- PHASE
- PHASESoundEvent
-  metaParameters 

Instance Property

# metaParameters

The object’s meta parameters.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var metaParameters: [String : PHASEMetaParameter] { get }
```

## Discussion

Each meta parameter contained in this dictionary affects only the sound event instance when you change the parameter’s value at runtime. As a read-only dictionary, the framework sets the contents based on the parameter you pass into a node definition initializer, for example, init(switchMetaParameterDefinition:). The dictionary key is the identifier of the source PHASEMetaParameterDefinition.

Tip

To propagate a metaparameter change to multiple sound events instead of just one, register the metaparameter globally by calling registerGlobalMetaParameter(metaParameterDefinition:). To change its value, access the metaparameter through the asset registry’s globalMetaParameters dictionary instead.

## See Also

### Configuring Mixers and Metaparameters

var mixers: [String : PHASEMixer]

Nodes in the event tree that control the volume of their child nodes.

