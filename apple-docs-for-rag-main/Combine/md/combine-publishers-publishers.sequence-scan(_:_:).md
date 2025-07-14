

- Combine
- Publishers
- Publishers.Sequence
-  scan(\_:\_:) 

Instance Method

# scan(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func scan(
    _ initialResult: T,
    _ nextPartialResult: @escaping (T, Publishers.Sequence.Output) -> T
) -> Publishers.Sequence
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

