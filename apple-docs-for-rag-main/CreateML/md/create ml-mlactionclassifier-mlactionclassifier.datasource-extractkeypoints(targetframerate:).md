

- Create ML
- MLActionClassifier
- MLActionClassifier.DataSource
-  extractKeypoints(targetFrameRate:) 

Instance Method

# extractKeypoints(targetFrameRate:)

Extracts key points from video files if necessary.

macOS 14.0+

``` source
func extractKeypoints(targetFrameRate: Double = MLHandActionClassifier.__Defaults.targetFrameRate) throws -> DataFrame
```

## Parameters 

`targetFrameRate`  

The number of frames per second the method uses to extract body landmarks from the data source.

## Return Value

A data frame that contains a column for hand joint locations and a column of hand action annotations.

## Discussion

If the data source already contains keypoints, this method just renames the data frame columns to the defaults.

## See Also

### Extracting key points

case labeledKeypointsDataFrame(DataFrame, sessionIdColumn: String, labelColumn: String, featureColumn: String)

A data source made up of keypoints in a data frame.

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

A data table that contains the human body landmark movement data.

Deprecated

case labeledVideoDataFrame(DataFrame, videoColumn: String, labelColumn: String, startTimeColumn: String?, endTimeColumn: String?)

A data source made up of video references in a data frame.

