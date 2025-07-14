

- Swift
- AnyBidirectionalCollection
-  init(\_:) 

Initializer

# init(\_:)

Creates an `AnyBidirectionalCollection` having the same underlying collection as `other`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(_ other: AnyCollection)
```

## Discussion

If the underlying collection stored by `other` does not satisfy `BidirectionalCollection`, the result is `nil`.

Complexity

O(1)

