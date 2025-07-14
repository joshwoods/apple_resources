

- Vision
- FeaturePrintObservation
-  distance(to:) 

Instance Method

# distance(to:)

Computes the distance between two feature print observations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func distance(to featurePrint: FeaturePrintObservation) throws -> Double
```

## Parameters 

`featurePrint`  

The feature print object to calculate the distance to.

## Return Value

The distance between two observations. Shorter distances indicate greater similarity between feature prints.

