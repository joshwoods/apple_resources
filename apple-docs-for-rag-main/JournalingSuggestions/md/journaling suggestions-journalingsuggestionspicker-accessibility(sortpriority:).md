

- Journaling Suggestions
- JournalingSuggestionsPicker
-  accessibility(sortPriority:) 

Instance Method

# accessibility(sortPriority:)

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

Journaling SuggestionsSwiftUIiOS 13.0–18.4DeprecatedmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func accessibility(sortPriority: Double) -> ModifiedContent
```

## Discussion

Higher numbers are sorted first. The default sort priority is zero.

