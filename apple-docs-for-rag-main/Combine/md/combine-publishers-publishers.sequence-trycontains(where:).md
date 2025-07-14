

- Combine
- Publishers
- Publishers.Sequence
-  tryContains(where:) 

Instance Method

# tryContains(where:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryContains(where predicate: (Publishers.Sequence.Output) throws -> Bool) -> Result.Publisher
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

