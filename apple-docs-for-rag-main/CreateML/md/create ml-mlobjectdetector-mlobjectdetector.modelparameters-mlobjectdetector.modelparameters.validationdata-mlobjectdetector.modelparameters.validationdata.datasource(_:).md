

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
- MLObjectDetector.ModelParameters.ValidationData
-  MLObjectDetector.ModelParameters.ValidationData.dataSource(\_:) 

Case

# MLObjectDetector.ModelParameters.ValidationData.dataSource(\_:)

A validation dataset you provide as a data source.

macOS 10.15+

``` source
case dataSource(MLObjectDetector.DataSource)
```

## Discussion

- dataSource : An MLObjectDetector.DataSource instance the enumeration case uses as its associated value.

## See Also

### Designating validation data

case split(strategy: MLSplitStrategy)

A validation dataset Create ML derives by randomly selecting a portion of the object detector’s training dataset using the split strategy.

case dataFrame(DataFrame, imageColumn: String, annotationColumn: String)

Set validation data from the MLDataTable provided.

case table(MLDataTable, imageColumn: String, annotationColumn: String)

A validation dataset you provide as a data table.

Deprecated

case none

An empty validation dataset that skips the model validation phase after training.

