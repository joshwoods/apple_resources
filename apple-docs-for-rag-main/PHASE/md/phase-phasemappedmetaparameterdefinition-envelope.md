

- PHASE
- PHASEMappedMetaParameterDefinition
-  envelope 

Instance Property

# envelope

A collection of line segments that curve and connect to form a graph.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var envelope: PHASEEnvelope { get }
```

## Discussion

The line segments collectively plot an output value for the inputMetaParameterDefinition property.

To plot the input, call evaluate(x:), passing in the input metaparameter’s value.

To gradually change the input over time, call fade(value:duration:).

