

- Create ML
- MLObjectDetector
- MLObjectDetector.DataSource
-  imagesWithObjectAnnotations() Deprecated

Instance Method

# imagesWithObjectAnnotations()

Generates a data table where each row represents an image, and its columns are the image file URLs and its annotations.

macOS 10.15–14.0Deprecated

``` source
func imagesWithObjectAnnotations() throws -> MLDataTable
```

Deprecated

Use gatherAnnotatedFileNames()

## Return Value

An MLDataTable containing the contents of the data source.

