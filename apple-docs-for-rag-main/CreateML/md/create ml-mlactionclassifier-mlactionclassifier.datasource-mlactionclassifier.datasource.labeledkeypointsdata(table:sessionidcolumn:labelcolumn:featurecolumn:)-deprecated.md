

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  MLActionClassifier.DataSource.labeledKeypointsData(table:sessionIdColumn:labelColumn:featureColumn:) Deprecated

Case

# MLActionClassifier.DataSource.labeledKeypointsData(table:sessionIdColumn:labelColumn:featureColumn:)

A data table that contains the human body landmark movement data.

macOS 11.0–14.0Deprecated

``` source
case labeledKeypointsData(
    table: MLDataTable,
    sessionIdColumn: String = __Defaults.sessionIdColumnName,
    labelColumn: String = __Defaults.labelColumnName,
    featureColumn: String = __Defaults.featureColumnName
)
```

## Parameters 

`table`  

A data table that contains the human body landmark locations and the action annotations.

`sessionIdColumn`  

The name of the column that contains the action session’s unique identifier.

`labelColumn`  

The name of the column that contains the labels of the action the person demonstrates in the session.

`featureColumn `  

The name of the column that contains the movement data.

## See Also

### Extracting key points

func extractKeypoints(targetFrameRate: Double) throws -> DataFrame

Extracts key points from video files if necessary.

case labeledKeypointsDataFrame(DataFrame, sessionIdColumn: String, labelColumn: String, featureColumn: String)

A data source made up of keypoints in a data frame.

case labeledVideoDataFrame(DataFrame, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

A data source made up of video references in a data frame.

