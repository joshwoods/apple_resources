

- SwiftData
- FetchResultsCollection
-  startIndex 

Instance Property

# startIndex

The position of the first element in a nonempty collection.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
var startIndex: Int { get }
```

## Discussion

If the collection is empty, `startIndex` is equal to `endIndex`.

## See Also

### Accessing indices

var endIndex: Int

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

