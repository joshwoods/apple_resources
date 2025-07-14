

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.DataSource
-  MLHandPoseClassifier.DataSource.labeledFiles(at:) 

Case

# MLHandPoseClassifier.DataSource.labeledFiles(at:)

Creates a data source from a folder that contains images, each named after the hand pose it represents.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case labeledFiles(at: URL)
```

## Discussion

Create a hand-pose data source from a directory of images with the `labeledFiles` case. You must name each image file with a hand-pose label, followed by a period and an arbitrary string, ending with the image file’s extension. For example, you can name a hand-pose classifier’s training files as `Peace.3.png`, `ThumbsUp.1.jpg`, `ThumbsUp.2.jpg`, and so on.

In this example, these image names give a hand-pose classifier at least two class labels:

- `Peace` - `ThumbsUp`

- at: The URL to a folder in the file system that contains folders of hand pose images. The data source uses each file’s name before the first period as its classification label.

## See Also

### Creating a data source

case labeledDirectories(at: URL)

Creates a data source from a folder with subfolders that each contain images of a hand pose.

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

