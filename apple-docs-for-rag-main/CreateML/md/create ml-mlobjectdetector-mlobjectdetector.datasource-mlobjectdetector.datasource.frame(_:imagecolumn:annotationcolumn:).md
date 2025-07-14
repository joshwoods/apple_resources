

- Create ML
- MLObjectDetector
- MLObjectDetector.DataSource
-  MLObjectDetector.DataSource.frame(\_:imageColumn:annotationColumn:) 

Case

# MLObjectDetector.DataSource.frame(\_:imageColumn:annotationColumn:)

Data specified by a `DataFrame` containing a column for image file paths and a column with annotations.

macOS 12.0+

``` source
case frame(
    DataFrame,
    imageColumn: String,
    annotationColumn: String
)
```

