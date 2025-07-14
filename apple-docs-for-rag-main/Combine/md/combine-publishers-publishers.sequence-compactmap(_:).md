

- Combine
- Publishers
- Publishers.Sequence
-  compactMap(\_:) 

Instance Method

# compactMap(\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func compactMap(_ transform: (Publishers.Sequence.Output) -> T?) -> Publishers.Sequence
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

