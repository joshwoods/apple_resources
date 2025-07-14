

- Create ML
- MLObjectDetector
-  init(trainingData:parameters:annotationType:) 

Initializer

# init(trainingData:parameters:annotationType:)

Creates an object detector with a data source.

macOS 10.15+

``` source
init(
    trainingData: MLObjectDetector.DataSource,
    parameters: MLObjectDetector.ModelParameters = .init(),
    annotationType: MLObjectDetector.AnnotationType
) throws
```

## Discussion

Use this initializer to create an object detector with an MLObjectDetector.DataSource.

- trainingData: A data source that contains the annotated images the task uses to train the object detector.

- annotationType : The format your data source uses for its image annotations.

## See Also

### Training an object detector synchronously

init(trainingData: MLDataTable, imageColumn: String, annotationColumn: String, annotationType: MLObjectDetector.AnnotationType, parameters: MLObjectDetector.ModelParameters) throws

Creates an object detector with a data table.

Deprecated

