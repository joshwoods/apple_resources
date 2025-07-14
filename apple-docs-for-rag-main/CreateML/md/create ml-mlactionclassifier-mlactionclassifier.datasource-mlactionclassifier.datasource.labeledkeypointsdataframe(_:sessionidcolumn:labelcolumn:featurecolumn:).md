

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  MLActionClassifier.DataSource.labeledKeypointsDataFrame(\_:sessionIdColumn:labelColumn:featureColumn:) 

Case

# MLActionClassifier.DataSource.labeledKeypointsDataFrame(\_:sessionIdColumn:labelColumn:featureColumn:)

A data source made up of keypoints in a data frame.

macOS 12.0+

``` source
case labeledKeypointsDataFrame(
    DataFrame,
    sessionIdColumn: String = __Defaults.sessionIdColumnName,
    labelColumn: String = __Defaults.labelColumnName,
    featureColumn: String = __Defaults.featureColumnName
)
```

## Parameters 

`dataFrame`  

A `DataFrame` containing keypoints and labels.

`sessionIdColumn`  

The name of the column containing session identifiers. Defaults to “session_id”.

`labelColumn`  

The name of the column containing the labels. Defaults to “label”.

`featureColumn`  

The name of the column containing the keypoints. Defaults to “keypoints”.

## Discussion

The data frame must contain a column of session identifiers, a column of labels, and a column of keypoints. Each set of keypoints must be a multi-dimensional 1x3x18 array containing the x, y, z coordinates of each of the 18 keypoints. See `VNRecognizedPointsObservation` for more details.

## See Also

### Extracting key points

func extractKeypoints(targetFrameRate: Double) throws -> DataFrame

Extracts key points from video files if necessary.

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

A data table that contains the human body landmark movement data.

Deprecated

case labeledVideoDataFrame(DataFrame, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

A data source made up of video references in a data frame.

