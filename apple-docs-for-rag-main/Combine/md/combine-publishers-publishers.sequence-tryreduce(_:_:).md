

- Combine
- Publishers
- Publishers.Sequence
-  tryReduce(\_:\_:) 

Instance Method

# tryReduce(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryReduce(
    _ initialResult: T,
    _ nextPartialResult: @escaping (T, Publishers.Sequence.Output) throws -> T
) -> Result.Publisher
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

