

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
- MLObjectDetector.ModelParameters.ValidationData
-  MLObjectDetector.ModelParameters.ValidationData.dataFrame(\_:imageColumn:annotationColumn:) 

Case

# MLObjectDetector.ModelParameters.ValidationData.dataFrame(\_:imageColumn:annotationColumn:)

Set validation data from the MLDataTable provided.

macOS 13.0+

``` source
case dataFrame(
    DataFrame,
    imageColumn: String,
    annotationColumn: String
)
```

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset Create ML derives by randomly selecting a portion of the object detector’s training dataset using the split strategy.

case dataSource(MLObjectDetector.DataSource)

A validation dataset you provide as a data source.

case table(MLDataTable, imageColumn: String, annotationColumn: String)

A validation dataset you provide as a data table.

Deprecated

case none

An empty validation dataset that skips the model validation phase after training.

