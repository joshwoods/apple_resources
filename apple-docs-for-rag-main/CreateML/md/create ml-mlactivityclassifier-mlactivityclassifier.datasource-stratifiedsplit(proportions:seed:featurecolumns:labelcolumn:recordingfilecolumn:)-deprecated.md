

- Create ML
- MLActivityClassifier
- MLActivityClassifier.DataSource
-  stratifiedSplit(proportions:seed:featureColumns:labelColumn:recordingFileColumn:) Deprecated

Instance Method

# stratifiedSplit(proportions:seed:featureColumns:labelColumn:recordingFileColumn:)

Generates a data table by splitting the data source into strata.

macOS 10.15–14.0Deprecated

``` source
func stratifiedSplit(
    proportions: [Double],
    seed: Int = timestampSeed(),
    featureColumns: [String],
    labelColumn: String,
    recordingFileColumn: String
) throws -> MLDataTable
```

Deprecated

Use DataFrame.stratifiedSplit(on:by:).

## Parameters 

`proportions`  

An array of proportions, each in the range `[0.0, 1.0]`.

`seed`  

A seed number for the random-number generator.

`featureColumns`  

The names of the feature columns the method includes in the data table.

`labelColumn`  

The name of the label column the methods stratifies.

`recordingFileColumn`  

The name of the column with the data file names.

## Return Value

A new MLDataTable instance.

## See Also

### Generating data tables from a data source

func labeledSensorData(featureColumns: [String], labelColumn: String?, recordingFileColumn: String?) throws -> MLDataTable

Generates a data table from the contents of the data source.

Deprecated

