

- Swift
- AsyncThrowingMapSequence
-  AsyncThrowingMapSequence.Failure 

Type Alias

# AsyncThrowingMapSequence.Failure

The type of error produced by this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Failure = any Error
```

Available when `Base` conforms to `AsyncSequence`.

## Discussion

The map sequence produces errors from either the base sequence or the `transform` closure.

