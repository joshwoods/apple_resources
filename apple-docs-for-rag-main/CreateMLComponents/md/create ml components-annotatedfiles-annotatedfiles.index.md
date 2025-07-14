

- Create ML Components
- AnnotatedFiles
-  AnnotatedFiles.Index 

Type Alias

# AnnotatedFiles.Index

A type that represents a position in the collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Index = Array.Index
```

## Discussion

Valid indices consist of the position of every element and a “past the end” position that’s not valid for use as a subscript argument.

## See Also

### Getting the index

func index(after: AnnotatedFiles.Index) -> AnnotatedFiles.Index

Returns the position immediately after the given index.

typealias Element

A type representing the sequence’s elements.

