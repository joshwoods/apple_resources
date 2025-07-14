

- Create ML
- MLObjectDetector
- MLObjectDetector.DataSource
-  MLObjectDetector.DataSource.directoryWithImages(at:annotationFile:) 

Case

# MLObjectDetector.DataSource.directoryWithImages(at:annotationFile:)

An object-detector data source you create by selecting the location of a directory of image files, and the location of a JSON annotation file.

macOS 10.15+

``` source
case directoryWithImages(
    at: URL,
    annotationFile: URL
)
```

## Discussion

- directoryWithImages: The location of a directory that contains image files.

- annotationFile: The location of a JSON file with object annotations for the images.

## See Also

### Creating a data source

case directoryWithImagesAndJsonAnnotation(at: URL)

An object-detector data source you create by selecting a directory that contains image files and exactly one JSON annotation file.

case table(MLDataTable, imageColumn: String, annotationColumn: String)

An object-detector data source you create with a data table.

Deprecated

