

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  MLHandPoseClassifier.DataSource.labeledDirectories(at:) 

Case

# MLHandPoseClassifier.DataSource.labeledDirectories(at:)

Creates a data source from a folder with subfolders that each contain images of a hand pose.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case labeledDirectories(at: URL)
```

## Discussion

- at: The URL to a folder in the file system that contains folders of hand pose images. The data source uses the name of each folder as the classification label for the hand pose images it contains.

## See Also

### Creating a data source

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

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data table of hand pose observations that each contain the locations of each hand joint and an annotation.

