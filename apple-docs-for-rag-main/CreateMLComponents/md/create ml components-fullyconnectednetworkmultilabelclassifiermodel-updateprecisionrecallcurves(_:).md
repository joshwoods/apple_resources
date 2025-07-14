

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifierModel
-  updatePrecisionRecallCurves(\_:) 

Instance Method

# updatePrecisionRecallCurves(\_:)

Updates the per-label precision-recall curve using the input data.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
mutating func updatePrecisionRecallCurves(_ input: some Collection, Set>>) async throws
```

## Parameters 

`input`  

A collection of annotated examples.

## Discussion

Call this method before exporting to a Core ML Model and using Vision `VNCoreMLRequest` to make predictions.

