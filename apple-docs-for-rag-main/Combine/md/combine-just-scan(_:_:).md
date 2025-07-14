

- Combine
- Just
-  scan(\_:\_:) 

Instance Method

# scan(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func scan(
    _ initialResult: T,
    _ nextPartialResult: (T, Output) -> T
) -> Result.Failure>.Publisher
```

## See Also

### Mapping Elements

func map&lt;T>((Output) -> T) -> Just&lt;T>

func tryMap&lt;T>((Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func mapError&lt;E>((Just&lt;Output>.Failure) -> E) -> Result&lt;Output, E>.Publisher

func replaceNil&lt;T>(with: T) -> Publishers.Map&lt;Self, T>

Replaces nil elements in the stream with the provided element.

func tryScan&lt;T>(T, (T, Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func setFailureType&lt;E>(to: E.Type) -> Result&lt;Output, E>.Publisher

