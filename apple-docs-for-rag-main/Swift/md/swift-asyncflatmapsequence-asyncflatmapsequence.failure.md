

- Swift
- AsyncFlatMapSequence
-  AsyncFlatMapSequence.Failure 

Type Alias

# AsyncFlatMapSequence.Failure

The type of error produced by this asynchronous sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
typealias Failure = Base.Failure
```

Available when `Base` conforms to `AsyncSequence` and `SegmentOfResult` conforms to `AsyncSequence`.

## Discussion

The flat map sequence produces the type of error in the base asynchronous sequence. By construction, the sequence produced by the `transform` closure must either produce this type of error or not produce errors at all.

