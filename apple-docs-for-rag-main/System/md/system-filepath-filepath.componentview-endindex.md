

- System
- FilePath
- FilePath.ComponentView
-  endIndex 

Instance Property

# endIndex

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var endIndex: FilePath.ComponentView.Index { get }
```

## Discussion

When you need a range that includes the last element of a collection, use the half-open range operator (`..

```
let numbers = [10, 20, 30, 40, 50]
if let index = numbers.firstIndex(of: 30) {
    print(numbers[index ..

If the collection is empty, `endIndex` is equal to `startIndex`.

