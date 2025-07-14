

- Combine
- Just
-  replaceError(with:) 

Instance Method

# replaceError(with:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func replaceError(with output: Output) -> Just
```

## See Also

### Filtering Elements

func filter((Output) -> Bool) -> Optional&lt;Output>.Publisher

func tryFilter((Self.Output) throws -> Bool) -> Publishers.TryFilter&lt;Self>

Republishes all elements that match a provided error-throwing closure.

func compactMap&lt;T>((Output) -> T?) -> Optional&lt;T>.Publisher

func tryCompactMap&lt;T>((Self.Output) throws -> T?) -> Publishers.TryCompactMap&lt;Self, T>

Calls an error-throwing closure with each received element and publishes any returned optional that has a value.

func removeDuplicates() -> Just&lt;Output>

func removeDuplicates(by: (Output, Output) -> Bool) -> Just&lt;Output>

func tryRemoveDuplicates(by: (Output, Output) throws -> Bool) -> Result&lt;Output, any Error>.Publisher

func replaceEmpty(with: Output) -> Just&lt;Output>

