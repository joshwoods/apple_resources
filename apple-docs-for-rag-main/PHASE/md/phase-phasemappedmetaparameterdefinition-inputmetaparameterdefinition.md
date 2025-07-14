

- PHASE
- PHASEMappedMetaParameterDefinition
-  inputMetaParameterDefinition 

Instance Property

# inputMetaParameterDefinition

A linear input value to plot on a curve.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var inputMetaParameterDefinition: PHASENumberMetaParameterDefinition { get }
```

## Discussion

This property defines the input value to plot on a graph defined by envelope.

To retrieve the output value, an app passes the metaparameter’s value to the evaluate(x:) function.

