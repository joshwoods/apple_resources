

- Journaling Suggestions
- JournalingSuggestion
- JournalingSuggestion.ItemContent
-  content(forType:) 

Instance Method

# content(forType:)

Retrieves a suggestion’s contents by returning a structure specific to the given content type.

iOS 17.2+

``` source
func content(forType content: Content.Type) async throws -> Content? where Content : JournalingSuggestionAsset
```

## Parameters 

`content`  

A type conforming to JournalingSuggestionAsset protocol.

## Return Value

An instance of the requested type, if it exists in the suggestion.

## Discussion

The framework templates this method, where `Content` is JournalingSuggestionAsset, because the `content` argument is a `Type` rather than an enumeration case, or other primitive.

Throws

An error if the journaling suggestions picker encounters an unexpected issue.

## See Also

### Accessing suggestion data by type

func hasContent&lt;Content>(ofType: Content.Type) -> Bool

Checks if the suggestion contains information for the given type.

