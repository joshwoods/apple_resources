

- Combine
- Publishers
- Publishers.Sequence
-  min(by:) 

Instance Method

# min(by:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func min(by areInIncreasingOrder: (Publishers.Sequence.Output, Publishers.Sequence.Output) -> Bool) -> Optional.Output>.Publisher
```

Available when `Elements` conforms to `Sequence` and `Failure` is `Never`.

