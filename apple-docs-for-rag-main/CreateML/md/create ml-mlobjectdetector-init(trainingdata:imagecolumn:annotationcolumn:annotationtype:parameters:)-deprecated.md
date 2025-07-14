

- Create ML
- MLObjectDetector
-  init(trainingData:imageColumn:annotationColumn:annotationType:parameters:) Deprecated

Initializer

# init(trainingData:imageColumn:annotationColumn:annotationType:parameters:)

Creates an object detector with a data table.

macOS 10.15–13.0Deprecated

``` source
init(
    trainingData: MLDataTable,
    imageColumn: String,
    annotationColumn: String,
    annotationType: MLObjectDetector.AnnotationType,
    parameters: MLObjectDetector.ModelParameters = ModelParameters()
) throws
```

Deprecated

Use DataSource instead of MLDataTable when initializing.

## Discussion

Use this initializer to create an object detector with an MLDataTable.

- trainingData: An MLDataTable that contains the annotated images the task uses to train the object detector.

- imageColumn: The name of the column in the data table that contains the image file URLs.

- annotationColumn: The name of the column in the data table that contains the image annotations.

- annotationType : The format your data table uses for its image annotations.

## See Also

### Training an object detector synchronously

init(trainingData: MLObjectDetector.DataSource, parameters: MLObjectDetector.ModelParameters, annotationType: MLObjectDetector.AnnotationType) throws

Creates an object detector with a data source.

