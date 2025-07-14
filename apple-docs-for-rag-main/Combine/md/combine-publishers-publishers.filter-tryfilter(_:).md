

- Combine
- Publishers
- Publishers.Filter
-  tryFilter(\_:) 

Instance Method

# tryFilter(\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryFilter(_ isIncluded: @escaping (Publishers.Filter.Output) throws -> Bool) -> Publishers.TryFilter
```

Available when `Upstream` conforms to `Publisher`.

## See Also

### Filtering Elements

func filter((Publishers.Filter&lt;Upstream>.Output) -> Bool) -> Publishers.Filter&lt;Upstream>

func compactMap&lt;T>((Self.Output) -> T?) -> Publishers.CompactMap&lt;Self, T>

Calls a closure with each received element and publishes any returned optional that has a value.

func tryCompactMap&lt;T>((Self.Output) throws -> T?) -> Publishers.TryCompactMap&lt;Self, T>

Calls an error-throwing closure with each received element and publishes any returned optional that has a value.

func removeDuplicates() -> Publishers.RemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element.

func removeDuplicates(by: (Self.Output, Self.Output) -> Bool) -> Publishers.RemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element, as evaluated by a provided closure.

func tryRemoveDuplicates(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryRemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

func replaceEmpty(with: Self.Output) -> Publishers.ReplaceEmpty&lt;Self>

Replaces an empty stream with the provided element.

func replaceError(with: Self.Output) -> Publishers.ReplaceError&lt;Self>

Replaces any errors in the stream with the provided element.

