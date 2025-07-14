

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  MLHandPoseClassifier.DataSource.labeledImageDataFrame(\_:imageColumn:labelColumn:) 

Case

# MLHandPoseClassifier.DataSource.labeledImageDataFrame(\_:imageColumn:labelColumn:)

Creates a data source from a data frame that contains the location and annotation for a set of image files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case labeledImageDataFrame(
    DataFrame,
    imageColumn: String = __Defaults.imageColumnName,
    labelColumn: String = __Defaults.labelColumnName
)
```

## Discussion

- dataFrame: A data frame that contains the locations of annotations for each hand pose image file.

- imageColumn: The name of the column in the data frame that contains the image filenames.

- labelColumn: The name of the column in the data frame that contains the hand pose label names.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain images of a hand pose.

case labeledFiles(at: URL)

Creates a data source from a folder that contains images, each named after the hand pose it represents.

case directoryWithImagesAndAnnotation(at: URL, annotationFile: URL, imageColumn: String, labelColumn: String)

Creates a data source from a folder that contains images and an annotation file.

case labeledKeypointsDataFrame(DataFrame, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data frame of hand pose observations that each contain the locations of each hand joint and an annotation.

case labeledImageData(table: MLDataTable, imageColumn: String, labelColumn: String)

Creates a data source from a data table that contains the hand joint locations and annotation for a set of image files.

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data table of hand pose observations that each contain the locations of each hand joint and an annotation.

