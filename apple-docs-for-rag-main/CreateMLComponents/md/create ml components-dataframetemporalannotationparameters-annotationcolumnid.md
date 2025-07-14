

- Create ML Components
- DataFrameTemporalAnnotationParameters
-  annotationColumnID 

Instance Property

# annotationColumnID

The column id that contains the annotation. The default value is “annotation” with `Annotation` type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var annotationColumnID: ColumnID
```

## See Also

### Getting the properties

var endTimeColumnID: ColumnID&lt;Double>?

The column id that contains the end time. The default value is `nil`.

var filePathColumnID: ColumnID&lt;String>

The column id that contains the file path. The default value is “filePath” with String type.

var filePathType: DataFrameTemporalAnnotationParameters&lt;Annotation>.FilePathType

The file path type in the annotation file. The default value is `.absolute`.

var startTimeColumnID: ColumnID&lt;Double>?

The column id that contains the start time. The default value is `nil`.

