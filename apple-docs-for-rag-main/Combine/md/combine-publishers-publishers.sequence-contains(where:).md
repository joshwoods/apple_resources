

- Combine
- Publishers
- Publishers.Sequence
-  contains(where:) 

Instance Method

# contains(where:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func contains(where predicate: (Publishers.Sequence.Output) -> Bool) -> Result.Publisher
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

