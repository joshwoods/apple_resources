

- Swift
- AnyBidirectionalCollection
-  count 

Instance Property

# count

The number of elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var count: Int { get }
```

## Discussion

To check whether a collection is empty, use its `isEmpty` property instead of comparing `count` to zero. Calculating `count` can be an O(*n*) operation.

Complexity

O(*n*)

