

- Swift
-  CustomPlaygroundQuickLookable 

Type Alias

# CustomPlaygroundQuickLookable

A type that explicitly supplies its own playground Quick Look.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias CustomPlaygroundQuickLookable = _CustomPlaygroundQuickLookable
```

## Discussion

The `CustomPlaygroundQuickLookable` protocol is deprecated, and will be removed from the standard library in a future Swift release. To customize the logging of your type in a playground, conform to the `CustomPlaygroundDisplayConvertible` protocol.

If you need to provide a customized playground representation in Swift 4.0 or Swift 3.2 or earlier, use a conditional compilation block:

```
#if swift(>=4.1) || (swift(>=3.3) && !swift(>=4.0))
    // With Swift 4.1 and later (including Swift 3.3 and later),
    // conform to CustomPlaygroundDisplayConvertible.
    extension MyType: CustomPlaygroundDisplayConvertible { /*...*/ }
#else
    // Otherwise, on Swift 4.0 and Swift 3.2 and earlier,
    // conform to CustomPlaygroundQuickLookable.
    extension MyType: CustomPlaygroundQuickLookable { /*...*/ }
#endif
```

## See Also

### Deprecated Type Aliases

typealias ArrayLiteralConvertible

typealias BidirectionalIndexable

typealias BidirectionalSlice

typealias BooleanLiteralConvertible

typealias ClosedRangeIndex

typealias DefaultBidirectionalIndices

typealias DefaultRandomAccessIndices

typealias DictionaryIterator

typealias DictionaryLiteralConvertible

typealias EmptyIterator

typealias ExtendedGraphemeClusterLiteralConvertible

typealias FlattenBidirectionalCollectionIndex

typealias FlattenBidirectionalCollection

typealias FlattenCollectionIndex

typealias FloatLiteralConvertible

