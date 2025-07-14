

- Create ML Components
-  DataFrameTemporalAnnotationParameters 

Structure

# DataFrameTemporalAnnotationParameters

Annotation parameters for the dataframe containing temporal annotations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct DataFrameTemporalAnnotationParameters where Annotation : Equatable, Annotation : Sendable
```

## Topics

### Creating the parameters

init()

Creates a DataFrameTemporalAnnotationParameters by using default options.

### Getting the properties

var annotationColumnID: ColumnID&lt;Annotation>

The column id that contains the annotation. The default value is “annotation” with `Annotation` type.

var endTimeColumnID: ColumnID&lt;Double>?

The column id that contains the end time. The default value is `nil`.

var filePathColumnID: ColumnID&lt;String>

The column id that contains the file path. The default value is “filePath” with String type.

var filePathType: DataFrameTemporalAnnotationParameters&lt;Annotation>.FilePathType

The file path type in the annotation file. The default value is `.absolute`.

var startTimeColumnID: ColumnID&lt;Double>?

The column id that contains the start time. The default value is `nil`.

### Specifying the path type

enum FilePathType

The file path type to be used.

## Relationships

### Conforms To

- Sendable

## See Also

### Annotations

struct AnnotatedFiles

An annotated files collection.

struct AnnotatedBatch

A batch of annotated examples for fitting a supervised estimator.

struct AnnotatedFeature

An annotated example for fitting a supervised estimator.

struct AnnotatedFeatureProvider

An adaptor that converts a regular estimator to a tabular estimator by selecting features and annotations from columns.

struct AnnotatedPrediction

An annotated prediction.

