

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
- MLObjectDetector.ModelParameters.ValidationData
-  MLObjectDetector.ModelParameters.ValidationData.none 

Case

# MLObjectDetector.ModelParameters.ValidationData.none

An empty validation dataset that skips the model validation phase after training.

macOS 10.15+

``` source
case none
```

## Discussion

Use this case when you don’t have validation data while preventing Create ML from using any of your training dataset for validation.

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset Create ML derives by randomly selecting a portion of the object detector’s training dataset using the split strategy.

case dataFrame(DataFrame, imageColumn: String, annotationColumn: String)

Set validation data from the MLDataTable provided.

case dataSource(MLObjectDetector.DataSource)

A validation dataset you provide as a data source.

case table(MLDataTable, imageColumn: String, annotationColumn: String)

A validation dataset you provide as a data table.

Deprecated

