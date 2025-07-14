

- Create ML Components
- AnnotatedBatch
-  init(features:annotations:) 

Initializer

# init(features:annotations:)

Creates an annotated batch.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    features: MLShapedArray,
    annotations: MLShapedArray
)
```

## Parameters 

`features`  

A shaped array of features.

`annotations`  

A shaped array of annotations.

## Discussion

The features and annotations must have the same rank, and the first dimensions must be equal.

