

- Swift
- Substring
-  endIndex 

Instance Property

# endIndex

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var endIndex: Substring.Index { get }
```

## Discussion

When you need a range that includes the last element of a collection, use the half-open range operator (`..

```
let numbers = [10, 20, 30, 40, 50]
if let index = numbers.firstIndex(of: 30) {
    print(numbers[index ..

If the collection is empty, `endIndex` is equal to `startIndex`.

