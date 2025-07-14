

- Swift
- AsyncDropFirstSequence
-  AsyncDropFirstSequence.Failure 

Type Alias

# AsyncDropFirstSequence.Failure

The type of errors produced by this asynchronous sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
typealias Failure = Base.Failure
```

Available when `Base` conforms to `AsyncSequence`.

## Discussion

The drop-first sequence produces whatever type of error its base sequence produces.

