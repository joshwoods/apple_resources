

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  MLHandPoseClassifier.DataSource.labeledImageData(table:imageColumn:labelColumn:) 

Case

# MLHandPoseClassifier.DataSource.labeledImageData(table:imageColumn:labelColumn:)

Creates a data source from a data table that contains the hand joint locations and annotation for a set of image files.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedvisionOS 1.0+

``` source
case labeledImageData(
    table: MLDataTable,
    imageColumn: String = __Defaults.imageColumnName,
    labelColumn: String = __Defaults.labelColumnName
)
```

## Discussion

- table: A data table that contains the locations of annotations for each hand pose image file.

- imageColumn: The name of the column in the data table that contains the image filenames.

- labelColumn: The name of the column in the data table that contains the hand pose label names.

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

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data table of hand pose observations that each contain the locations of each hand joint and an annotation.

