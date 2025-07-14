

- Create ML
- MLObjectDetector
- MLObjectDetector.DataSource
-  MLObjectDetector.DataSource.table(\_:imageColumn:annotationColumn:) Deprecated

Case

# MLObjectDetector.DataSource.table(\_:imageColumn:annotationColumn:)

An object-detector data source you create with a data table.

macOS 11.0–14.0Deprecated

``` source
case table(
    MLDataTable,
    imageColumn: String,
    annotationColumn: String
)
```

## Discussion

- table: An MLDataTable instance that contains a column of image file locations and a column of object annotations.

- imageColumn: The name of the column in the data table that contains the URL for an image.

- annotationColumn: The name of the column in the data table that contains the object annotations for an image.

## See Also

### Creating a data source

case directoryWithImagesAndJsonAnnotation(at: URL)

An object-detector data source you create by selecting a directory that contains image files and exactly one JSON annotation file.

case directoryWithImages(at: URL, annotationFile: URL)

An object-detector data source you create by selecting the location of a directory of image files, and the location of a JSON annotation file.

