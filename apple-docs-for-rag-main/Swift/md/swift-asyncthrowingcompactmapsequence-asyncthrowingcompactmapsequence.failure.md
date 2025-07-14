

- Swift
- AsyncThrowingCompactMapSequence
-  AsyncThrowingCompactMapSequence.Failure 

Type Alias

# AsyncThrowingCompactMapSequence.Failure

The type of element produced by this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Failure = any Error
```

Available when `Base` conforms to `AsyncSequence`.

## Discussion

The compact map sequence produces errors from either the base sequence or the transforming closure.

