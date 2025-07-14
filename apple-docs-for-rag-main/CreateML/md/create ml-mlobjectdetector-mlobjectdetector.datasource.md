

- Create ML
- MLObjectDetector
-  MLObjectDetector.DataSource 

Enumeration

# MLObjectDetector.DataSource

A data source for an object detector.

macOS 10.15+

``` source
enum DataSource
```

## Overview

You use a data source to specify the training dataset for an MLObjectDetector training session. An object-detector data source represents a set of images and an annotation for each object in an image.

Each object annotation consists of the object’s name, or *label*, and its location in the image. A single image can have multiple objects and, therefore, multiple annotations. For example, you can train an object detector with images of dining tables, along with annotations for bananas, croissants, and beverages. Each image can have one or more instances of an object, or any combination of objects.

## Topics

### Creating a data source

case directoryWithImagesAndJsonAnnotation(at: URL)

An object-detector data source you create by selecting a directory that contains image files and exactly one JSON annotation file.

case directoryWithImages(at: URL, annotationFile: URL)

An object-detector data source you create by selecting the location of a directory of image files, and the location of a JSON annotation file.

case table(MLDataTable, imageColumn: String, annotationColumn: String)

An object-detector data source you create with a data table.

Deprecated

### Getting the annotated file names

func gatherAnnotatedFileNames() throws -> DataFrame

Processes the data source and returns a data frame that contains file URLs and annotations.

### Getting the data frame

case frame(DataFrame, imageColumn: String, annotationColumn: String)

Data specified by a `DataFrame` containing a column for image file paths and a column with annotations.

### Retrieving the data

func imagesWithObjectAnnotations() throws -> MLDataTable

Generates a data table where each row represents an image, and its columns are the image file URLs and its annotations.

Deprecated

### Splitting the data

func stratifiedSplit(proportions: [Double], seed: Int, annotationColumn: String) throws -> MLDataTable

Generates a new data table by splitting the data source using the specified proportions.

Deprecated

## See Also

### Supporting types

enum AnnotationType

The available types of image annotations.

struct ModelParameters

Parameters that affect the process of training an object detection model.

