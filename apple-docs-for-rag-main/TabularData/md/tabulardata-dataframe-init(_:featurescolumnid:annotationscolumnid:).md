

- TabularData
- DataFrame
-  init(\_:featuresColumnID:annotationsColumnID:) 

Initializer

# init(\_:featuresColumnID:annotationsColumnID:)

Creates a data frame from a sequence of annotated features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    _ sequence: S,
    featuresColumnID: ColumnID,
    annotationsColumnID: ColumnID
) throws where S : Sequence, S.Element == AnnotatedFeature
```

## Discussion

- Parameters

  - featuresColumnID: The features column ID in the data frame.

  - annotationsColumnID: The annotations column ID in the data frame.

