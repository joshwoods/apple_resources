

- SwiftData
- FetchResultsCollection
-  endIndex 

Instance Property

# endIndex

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
var endIndex: Int { get }
```

## Discussion

When you need a range that includes the last element of a collection, use the half-open range operator (`..

```
let numbers = [10, 20, 30, 40, 50]
if let index = numbers.firstIndex(of: 30) {
    print(numbers[index ..

If the collection is empty, `endIndex` is equal to `startIndex`.

## See Also

### Accessing indices

var startIndex: Int

The position of the first element in a nonempty collection.

