

- Create ML Components
- AnnotatedFiles
-  startIndex 

Instance Property

# startIndex

The position of the first element in a nonempty collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var startIndex: AnnotatedFiles.Index { get }
```

## Discussion

If the collection is empty, `startIndex` is equal to `endIndex`.

## See Also

### Getting the properties

var endIndex: AnnotatedFiles.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

