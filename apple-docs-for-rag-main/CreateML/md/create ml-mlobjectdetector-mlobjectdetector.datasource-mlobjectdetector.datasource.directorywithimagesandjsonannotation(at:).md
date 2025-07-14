

- Create ML
- MLObjectDetector
- MLObjectDetector.DataSource
-  MLObjectDetector.DataSource.directoryWithImagesAndJsonAnnotation(at:) 

Case

# MLObjectDetector.DataSource.directoryWithImagesAndJsonAnnotation(at:)

An object-detector data source you create by selecting a directory that contains image files and exactly one JSON annotation file.

macOS 10.15+

``` source
case directoryWithImagesAndJsonAnnotation(at: URL)
```

## Discussion

- directoryWithImagesAndJsonAnnotation: The location of a directory that contains exactly one JSON annotation file and all the image files the JSON file’s annotations refer to.

## See Also

### Creating a data source

case directoryWithImages(at: URL, annotationFile: URL)

An object-detector data source you create by selecting the location of a directory of image files, and the location of a JSON annotation file.

case table(MLDataTable, imageColumn: String, annotationColumn: String)

An object-detector data source you create with a data table.

Deprecated

