

- Swift
- AsyncFlatMapSequence
-  AsyncFlatMapSequence.Element 

Type Alias

# AsyncFlatMapSequence.Element

The type of element produced by this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Element = SegmentOfResult.Element
```

Available when `Base` conforms to `AsyncSequence` and `SegmentOfResult` conforms to `AsyncSequence`.

## Discussion

The flat map sequence produces the type of element in the asynchronous sequence produced by the `transform` closure.

