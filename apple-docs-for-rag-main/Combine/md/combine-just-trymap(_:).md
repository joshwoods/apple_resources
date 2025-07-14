

- Combine
- Just
-  tryMap(\_:) 

Instance Method

# tryMap(\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryMap(_ transform: (Output) throws -> T) -> Result.Publisher
```

## See Also

### Mapping Elements

func map&lt;T>((Output) -> T) -> Just&lt;T>

func mapError&lt;E>((Just&lt;Output>.Failure) -> E) -> Result&lt;Output, E>.Publisher

func replaceNil&lt;T>(with: T) -> Publishers.Map&lt;Self, T>

Replaces nil elements in the stream with the provided element.

func scan&lt;T>(T, (T, Output) -> T) -> Result&lt;T, Just&lt;Output>.Failure>.Publisher

func tryScan&lt;T>(T, (T, Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func setFailureType&lt;E>(to: E.Type) -> Result&lt;Output, E>.Publisher

