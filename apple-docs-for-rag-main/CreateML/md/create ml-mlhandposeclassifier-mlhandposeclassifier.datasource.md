

- Create ML
- MLHandPoseClassifier
-  MLHandPoseClassifier.DataSource 

Enumeration

# MLHandPoseClassifier.DataSource

A hand pose classifier dataset that contains annotated images or hand joint location data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
enum DataSource
```

## Topics

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

case labeledKeypointsData(table: MLDataTable, sessionIdColumn: String, labelColumn: String, featureColumn: String)

Creates a data source from a data table of hand pose observations that each contain the locations of each hand joint and an annotation.

### Extracting keypoints

func extractKeypoints() throws -> DataFrame

Extracts key points from video files if necessary.

### Getting annotated file names

func gatherAnnotatedFileNames() throws -> DataFrame?

Processes the data source and returns a data frame that contains file URLs and annotations.

### Exporting a data source

func labeledMedia() throws -> [String : [URL]]

Generates a dictionary that contains the data source’s classification labels paired with an array of URLs to the label’s image files.

func imagesWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for the data source’s image file URLs and a column of annotations.

Deprecated

func keypointsWithAnnotations() throws -> MLDataTable

Generates a data table that contains a column for hand joint locations and hand pose annotations.

Deprecated

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

Deprecated

## See Also

### Supporting types

struct ModelParameters

A set of parameters that affect the training process of a hand pose classifier task.

