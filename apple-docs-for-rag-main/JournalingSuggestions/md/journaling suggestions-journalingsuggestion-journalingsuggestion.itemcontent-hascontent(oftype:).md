

- Journaling Suggestions
- JournalingSuggestion
- JournalingSuggestion.ItemContent
-  hasContent(ofType:) 

Instance Method

# hasContent(ofType:)

Checks if the suggestion contains information for the given type.

iOS 17.2+

``` source
func hasContent(ofType content: Content.Type) -> Bool where Content : JournalingSuggestionAsset
```

## Parameters 

`content`  

The type of information to check for.

## Return Value

`true`, if the suggestion contains information for the given type; otherwise, `false`.

## Discussion

The framework templates this method, where `Content` is JournalingSuggestionAsset, because the `content` argument is a `Type` rather than an enumeration case, or other primitive.

## See Also

### Accessing suggestion data by type

func content&lt;Content>(forType: Content.Type) async throws -> Content?

Retrieves a suggestion’s contents by returning a structure specific to the given content type.

