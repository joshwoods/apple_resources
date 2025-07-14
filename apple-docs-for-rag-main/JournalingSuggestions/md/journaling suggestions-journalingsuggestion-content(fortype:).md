

- Journaling Suggestions
- JournalingSuggestion
-  content(forType:) 

Instance Method

# content(forType:)

Searches a suggestion’s items for information of the given type.

iOS 17.2+

``` source
func content(forType content: Content.Type) async -> [Content] where Content : JournalingSuggestionAsset
```

## Parameters 

`content`  

A type that conforms to the JournalingSuggestionAsset protocol.

## Return Value

An array that contains elements of the requested type, if they exist in the suggestion.

## Discussion

The framework templates this method, where `Content` is JournalingSuggestionAsset, because the `content` argument is a `Type` rather than an enumeration case, or other primitive.

Throws

An error if the journaling suggestions picker encounters an unexpected issue.

## See Also

### Accessing suggestion data by type

let items: [JournalingSuggestion.ItemContent]

The individual items that compose the suggestion’s content.

struct ItemContent

A container for the information about a specific suggestion.

