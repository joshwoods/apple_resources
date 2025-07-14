

- Swift
- Int
- Int.Words
-  underestimatedCount 

Instance Property

# underestimatedCount

A value less than or equal to the number of elements in the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var underestimatedCount: Int { get }
```

## Discussion

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

