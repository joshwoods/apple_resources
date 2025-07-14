

- SwiftData
- FetchResultsCollection
-  underestimatedCount 

Instance Property

# underestimatedCount

A value less than or equal to the number of elements in the collection.

SwiftDataSwiftiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var underestimatedCount: Int { get }
```

## Discussion

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

