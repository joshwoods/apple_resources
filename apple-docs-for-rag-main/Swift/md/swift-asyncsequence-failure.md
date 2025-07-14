

- Swift
- AsyncSequence
-  Failure 

Associated Type

# Failure

The type of errors produced when iteration over the sequence fails.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
associatedtype Failure = any Error where Self.Failure == Self.AsyncIterator.Failure
```

**Required**

