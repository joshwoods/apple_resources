

- Swift
- AsyncMapSequence
-  AsyncMapSequence.Element 

Type Alias

# AsyncMapSequence.Element

The type of element produced by this asynchronous sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Element = Transformed
```

Available when `Base` conforms to `AsyncSequence`.

## Discussion

The map sequence produces whatever type of element its transforming closure produces.

