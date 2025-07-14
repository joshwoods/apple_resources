

- Create ML Components
-  AnnotatedFiles 

Structure

# AnnotatedFiles

An annotated files collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct AnnotatedFiles
```

## Topics

### Creating the feature

init(labeledBySubdirectoryNamesAt: URL, type: UTType, continueOnFailure: Bool) throws

Reads training examples from a directory containing files in labeled sub-directories.

init(labeledByNamesAt: URL, separator: Character, index: Int, type: UTType, continueOnFailure: Bool) throws

Reads training examples from a directory containing files having their labels in the name. The name can contain multiple words separated by a `separator`. So the `index` tells the position of the label in the file name. Files with incorrect name format are ignored.

### Getting the properties

var endIndex: AnnotatedFiles.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: AnnotatedFiles.Index

The position of the first element in a nonempty collection.

### Getting the index

func index(after: AnnotatedFiles.Index) -> AnnotatedFiles.Index

Returns the position immediately after the given index.

typealias Index

A type that represents a position in the collection.

typealias Element

A type representing the sequence’s elements.

### Accessing by subscript

subscript(AnnotatedFiles.Index) -> IndexingIterator&lt;AnnotatedFiles>.Element

Accesses the element at the specified position.

### Type Aliases

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

Collection Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- Sequence

## See Also

### Annotations

struct AnnotatedBatch

A batch of annotated examples for fitting a supervised estimator.

struct AnnotatedFeature

An annotated example for fitting a supervised estimator.

struct AnnotatedFeatureProvider

An adaptor that converts a regular estimator to a tabular estimator by selecting features and annotations from columns.

struct AnnotatedPrediction

An annotated prediction.

struct DataFrameTemporalAnnotationParameters

Annotation parameters for the dataframe containing temporal annotations.

