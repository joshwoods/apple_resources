

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  MLHandPoseClassifier.DataSource.labeledKeypointsData(table:sessionIdColumn:labelColumn:featureColumn:) 

Case

# MLHandPoseClassifier.DataSource.labeledKeypointsData(table:sessionIdColumn:labelColumn:featureColumn:)

Creates a data source from a data table of hand pose observations that each contain the locations of each hand joint and an annotation.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedvisionOS 1.0+

``` source
case labeledKeypointsData(
    table: MLDataTable,
    sessionIdColumn: String = __Defaults.sessionIdColumnName,
    labelColumn: String = __Defaults.labelColumnName,
    featureColumn: String = __Defaults.featureColumnName
)
```

## Discussion

- table : A data table that contains the hand-joint locations and annotations for a set of hand poses.

- sessionIdColumn: The name of the column in the data table that contains the session identifiers.

- labelColumn: The name of the column in the data table that contains the hand pose label names.

- featureColumn: The name of the column in the data table that contains the hand-joint location data. Each entry in the column must be an MLMultiArray instance — which you must wrap in an MLDataValue.MultiArrayType — that contains three dimensions:

  - The first dimension has a size of one.

- The second dimension has three channels: the x-coordinate, the y-coordinate, and the confidence value, respectively. - The third dimension has 21 channels, one for each hand joint.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain images of a hand pose.

case labeledFiles(at: URL)

Creates a data source from a folder that contains images, each named after the hand pose it represents.

case directoryWithImagesAndAnnotation(at: URL, annotationFile: URL, imageColumn: String, labelColumn: String)

Creates a data source from a folder that contains images and an annotation file.

case labeledImageDataFrame(DataFrame, imageColumn: String, labelColumn: String)

Creates a data source from a data frame that contains the location and annotation for a set of image files.

case labeledKeypointsDataFrame(DataFrame, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data frame of hand pose observations that each contain the locations of each hand joint and an annotation.

case labeledImageData(table: MLDataTable, imageColumn: String, labelColumn: String)

Creates a data source from a data table that contains the hand joint locations and annotation for a set of image files.

