

- Create ML Components
- AnnotatedFiles
-  endIndex 

Instance Property

# endIndex

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var endIndex: AnnotatedFiles.Index { get }
```

## Discussion

When you need a range that includes the last element of a collection, use the half-open range operator (`..

```
let numbers = [10, 20, 30, 40, 50]
if let index = numbers.firstIndex(of: 30) {
    print(numbers[index ..

If the collection is empty, `endIndex` is equal to `startIndex`.

## See Also

### Getting the properties

var startIndex: AnnotatedFiles.Index

The position of the first element in a nonempty collection.

