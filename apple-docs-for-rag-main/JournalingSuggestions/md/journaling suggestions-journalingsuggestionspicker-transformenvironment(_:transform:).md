

- Journaling Suggestions
- JournalingSuggestionsPicker
-  transformEnvironment(\_:transform:) 

Instance Method

# transformEnvironment(\_:transform:)

Transforms the environment value of the specified key path with the given function.

Journaling SuggestionsSwiftUIiOS 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func transformEnvironment(
    _ keyPath: WritableKeyPath,
    transform: @escaping (inout V) -> Void
) -> some View
```

