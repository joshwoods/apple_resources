

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  extractKeypoints() 

Instance Method

# extractKeypoints()

Extracts key points from video files if necessary.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func extractKeypoints() throws -> DataFrame
```

## Return Value

A data frame that contains a column for hand joint locations and a column of hand action annotations.

## Discussion

If the data source already contains keypoints, this method just renames the data frame columns to the defaults.

