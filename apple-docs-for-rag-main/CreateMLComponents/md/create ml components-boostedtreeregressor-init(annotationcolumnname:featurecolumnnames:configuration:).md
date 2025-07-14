

- Create ML Components
- BoostedTreeRegressor
-  init(annotationColumnName:featureColumnNames:configuration:) 

Initializer

# init(annotationColumnName:featureColumnNames:configuration:)

Creates a boosted tree regressor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    annotationColumnName: String,
    featureColumnNames: [String],
    configuration: BoostedTreeConfiguration = BoostedTreeConfiguration()
)
```

## Discussion

- Parameters

  - annotationColumnName: The name of the column containing the ground truth values.

  - featureColumnNames: The names of the feature columns.

  - configuration: The configuration.

