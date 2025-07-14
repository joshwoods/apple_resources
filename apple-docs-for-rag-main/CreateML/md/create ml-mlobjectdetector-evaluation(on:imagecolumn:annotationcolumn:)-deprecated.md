

- Create ML
- MLObjectDetector
-  evaluation(on:imageColumn:annotationColumn:) Deprecated

Instance Method

# evaluation(on:imageColumn:annotationColumn:)

Generates metrics by evaluating the object detector’s performance using annotated images in a data table.

macOS 10.15–13.0Deprecated

``` source
func evaluation(
    on annotatedImages: MLDataTable,
    imageColumn: String,
    annotationColumn: String
) -> MLObjectDetectorMetrics
```

Deprecated

Use DataSource instead of MLDataTable.

## Parameters 

`annotatedImages`  

An MLDataTable instance that contains a set of images with object annotations.

`imageColumn`  

The name of the column in the data table that contains the image file URLs.

`annotationColumn`  

The name of the column in the data table that contains the object annotations.

## Return Value

An MLObjectDetectorMetrics instance that represents the object detector’s performance on the annotated images.

## See Also

### Evaluating an object detector

func evaluation(on: MLObjectDetector.DataSource) -> MLObjectDetectorMetrics

Generates metrics by evaluating the object detector’s performance using annotated images in a data source.

