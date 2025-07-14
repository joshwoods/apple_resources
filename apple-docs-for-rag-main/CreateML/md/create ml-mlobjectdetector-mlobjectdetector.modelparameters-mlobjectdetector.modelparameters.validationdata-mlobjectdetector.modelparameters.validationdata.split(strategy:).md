

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
- MLObjectDetector.ModelParameters.ValidationData
-  MLObjectDetector.ModelParameters.ValidationData.split(strategy:) 

Case

# MLObjectDetector.ModelParameters.ValidationData.split(strategy:)

A validation dataset Create ML derives by randomly selecting a portion of the object detector’s training dataset using the split strategy.

macOS 10.15+

``` source
case split(strategy: MLSplitStrategy)
```

## Discussion

- strategy: An MLSplitStrategy instance the enumeration case uses to select a portion of the object detector’s training dataset as its associated value.

## See Also

### Designating validation data

case dataFrame(DataFrame, imageColumn: String, annotationColumn: String)

Set validation data from the MLDataTable provided.

case dataSource(MLObjectDetector.DataSource)

A validation dataset you provide as a data source.

case table(MLDataTable, imageColumn: String, annotationColumn: String)

A validation dataset you provide as a data table.

Deprecated

case none

An empty validation dataset that skips the model validation phase after training.

