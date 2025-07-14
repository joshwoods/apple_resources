

- Vision
- VNFeaturePrintObservation
-  computeDistance(\_:to:) 

Instance Method

# computeDistance(\_:to:)

Computes the distance between two feature print observations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func computeDistance(
    _ outDistance: UnsafeMutablePointer,
    to featurePrint: VNFeaturePrintObservation
) throws
```

## Parameters 

`outDistance`  

A pointer to store the calculated distance value.

`featurePrint`  

The feature print object whose distance to calculate.

## Discussion

Shorter distances indicate greater similarity between feature prints.

