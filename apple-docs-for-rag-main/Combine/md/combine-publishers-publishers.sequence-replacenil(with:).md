

- Combine
- Publishers
- Publishers.Sequence
-  replaceNil(with:) 

Instance Method

# replaceNil(with:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func replaceNil(with output: T) -> Publishers.Sequence.Output], Failure> where Elements.Element == T?
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

