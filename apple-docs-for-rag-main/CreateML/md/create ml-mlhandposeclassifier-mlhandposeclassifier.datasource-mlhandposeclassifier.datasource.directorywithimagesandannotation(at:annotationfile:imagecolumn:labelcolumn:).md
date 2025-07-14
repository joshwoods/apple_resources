

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  MLHandPoseClassifier.DataSource.directoryWithImagesAndAnnotation(at:annotationFile:imageColumn:labelColumn:) 

Case

# MLHandPoseClassifier.DataSource.directoryWithImagesAndAnnotation(at:annotationFile:imageColumn:labelColumn:)

Creates a data source from a folder that contains images and an annotation file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case directoryWithImagesAndAnnotation(
    at: URL,
    annotationFile: URL,
    imageColumn: String,
    labelColumn: String
)
```

## Parameters 

`at`  

A URL to a folder in the file system that contains images.

## Discussion

- annotationFile: A URL to a JSON or CSV file that contains annotations for the hand pose images.

- imageColumn: The name of the column or key name in the annotation file that contains the image filenames.

- labelColumn: The name of the column or key name in the annotation file that contains the hand pose label names.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain images of a hand pose.

case labeledFiles(at: URL)

Creates a data source from a folder that contains images, each named after the hand pose it represents.

case labeledImageDataFrame(DataFrame, imageColumn: String, labelColumn: String)

Creates a data source from a data frame that contains the location and annotation for a set of image files.

case labeledKeypointsDataFrame(DataFrame, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data frame of hand pose observations that each contain the locations of each hand joint and an annotation.

case labeledImageData(table: MLDataTable, imageColumn: String, labelColumn: String)

Creates a data source from a data table that contains the hand joint locations and annotation for a set of image files.

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data table of hand pose observations that each contain the locations of each hand joint and an annotation.

