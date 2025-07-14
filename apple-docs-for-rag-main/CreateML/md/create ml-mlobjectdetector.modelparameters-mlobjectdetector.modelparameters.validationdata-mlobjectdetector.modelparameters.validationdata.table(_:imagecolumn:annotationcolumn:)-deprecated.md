

- Create ML
- MLObjectDetector
- 
  - MLObjectDetector
- MLObjectDetector.ModelParameters
- MLObjectDetector.ModelParameters.ValidationData
-  MLObjectDetector.ModelParameters.ValidationData.table(\_:imageColumn:annotationColumn:) Deprecated

Case

# MLObjectDetector.ModelParameters.ValidationData.table(\_:imageColumn:annotationColumn:)

A validation dataset you provide as a data table.

macOS 10.15–14.0Deprecated

``` source
case table(
    MLDataTable,
    imageColumn: String,
    annotationColumn: String
)
```

## Discussion

- table : An MLDataTable instance the enumeration case uses as its associated value.

- imageColumn: The name of the column in the data table that contains the image file URLs.

- annotationColumn : The name of the column in the data table that contains the image annotations.

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset Create ML derives by randomly selecting a portion of the object detector’s training dataset using the split strategy.

case dataFrame(DataFrame, imageColumn: String, annotationColumn: String)

Set validation data from the MLDataTable provided.

case dataSource(MLObjectDetector.DataSource)

A validation dataset you provide as a data source.

case none

An empty validation dataset that skips the model validation phase after training.

