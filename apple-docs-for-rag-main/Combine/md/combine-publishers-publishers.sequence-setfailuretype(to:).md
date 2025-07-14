

- Combine
- Publishers
- Publishers.Sequence
-  setFailureType(to:) 

Instance Method

# setFailureType(to:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setFailureType(to error: E.Type) -> Publishers.Sequence where E : Error
```

Available when `Elements` conforms to `Sequence` and `Failure` conforms to `Error`.

