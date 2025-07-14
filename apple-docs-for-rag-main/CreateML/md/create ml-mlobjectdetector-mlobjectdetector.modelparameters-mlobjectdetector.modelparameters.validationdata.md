

- Create ML
- MLObjectDetector
- MLObjectDetector.ModelParameters
-  MLObjectDetector.ModelParameters.ValidationData 

Enumeration

# MLObjectDetector.ModelParameters.ValidationData

A validation dataset for an object detector.

macOS 10.15+

``` source
enum ValidationData
```

## Topics

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

case none

An empty validation dataset that skips the model validation phase after training.

## See Also

### Supporting types

enum ModelAlgorithmType

An object-detector training algorithm.

