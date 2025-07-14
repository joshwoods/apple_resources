

- TabularData
- DataFrame
-  loadRangedAnnotations(parameters:continueOnFailure:) 

Instance Method

# loadRangedAnnotations(parameters:continueOnFailure:)

Loads training examples from a data frame containing annotations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func loadRangedAnnotations(
    parameters: DataFrameTemporalAnnotationParameters = .init(),
    continueOnFailure: Bool = false
) throws -> [AnnotatedFeature] where Annotation : Equatable, Annotation : Sendable
```

## Parameters 

`parameters`  

Annotation parameters for using specific column names from the data frame. By default the data frame is expected to have columns `filePath` and `annotation`.

`continueOnFailure`  

A Boolean value indicating whether to continue reading the dataframe after encountering a row that is invalid. The default value is `false`.

## Return Value

A list of annotated features containing `URLRange` as feature and `Annotation` as annotation.

## Discussion

The exact column ids within the data frame which contains the file path, annotation, startTime and endTime of each temporal annotation, can be customized using the `parameters` argument.

The data frame must contain at least two columns: one for file path and one for annotation. The file path must be of String type and annotation can be of any equatable type.

The `filePath` column in the `dataFrame` should contain file path with its extension. All the files can have absolute path or a path relative to a `baseURL`. This option can be specified using `filePathType` in `parameters`.

The `startTime` and `endTime` columns contain the start time and end time of a temporal segment in seconds. Their type is Double. Both the columns are optional.

If only a `startTime` is specified, it is interpreted as an annotation for the range starting from `startTime` till the end of file, i.e., `startTime ...`.

If only an `endTime` is specified, it is interpreted as an annotation for the range starting at 0 till `endTime`, i.e., `0 ..

```
------------------------------------------------
| fileName  | annotation | startTime | endTime |
| ----------|------------|-----------|---------|
| file1.wav |   class1   |     0     |   4     |
| file1.wav |   class2   |     5     |   10    |
| file2.wav |   class1   |     2     |         |
| file3.wav |   class2   |           |         |
| file4.wav |   class1   |           |   5     |
------------------------------------------------
```

This will create an annotated feature list which has the following structure:

```
[
    AnnotatedFeature(feature:  TemporalFileSegment("file1.wav", 0 ..

