

- Create ML
- MLObjectDetector
-  evaluation(on:) 

Instance Method

# evaluation(on:)

Generates metrics by evaluating the object detector’s performance using annotated images in a data source.

macOS 10.15+

``` source
func evaluation(on annotatedImages: MLObjectDetector.DataSource) -> MLObjectDetectorMetrics
```

## Parameters 

`annotatedImages`  

An MLObjectDetector.DataSource instance that contains a set of images with object annotations.

## Return Value

An MLObjectDetectorMetrics instance that represents the object detector’s performance on the annotated images.

## See Also

### Evaluating an object detector

func evaluation(on: MLDataTable, imageColumn: String, annotationColumn: String) -> MLObjectDetectorMetrics

Generates metrics by evaluating the object detector’s performance using annotated images in a data table.

Deprecated

