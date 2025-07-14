

- Journaling Suggestions
- JournalingSuggestion
-  items 

Instance Property

# items

The individual items that compose the suggestion’s content.

iOS 17.2+

``` source
let items: [JournalingSuggestion.ItemContent]
```

## Mentioned in 

Presenting the suggestions picker and processing a selection

## See Also

### Accessing suggestion data by type

struct ItemContent

A container for the information about a specific suggestion.

func content&lt;Content>(forType: Content.Type) async -> [Content]

Searches a suggestion’s items for information of the given type.

