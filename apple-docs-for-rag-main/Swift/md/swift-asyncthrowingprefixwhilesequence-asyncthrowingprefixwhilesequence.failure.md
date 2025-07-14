

- Swift
- AsyncThrowingPrefixWhileSequence
-  AsyncThrowingPrefixWhileSequence.Failure 

Type Alias

# AsyncThrowingPrefixWhileSequence.Failure

The type of error produced by this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Failure = any Error
```

Available when `Base` conforms to `AsyncSequence`.

## Discussion

The prefix-while sequence produces errors from either the base sequence or the filtering closure.

