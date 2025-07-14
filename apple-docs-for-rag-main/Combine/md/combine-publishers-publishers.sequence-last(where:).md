

- Combine
- Publishers
- Publishers.Sequence
-  last(where:) 

Instance Method

# last(where:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func last(where predicate: (Publishers.Sequence.Output) -> Bool) -> Optional.Output>.Publisher
```

Available when `Elements` conforms to `BidirectionalCollection` and `Failure` is `Never`.

