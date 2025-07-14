

- Journaling Suggestions
- JournalingSuggestionsPicker
-  onLongPressGesture(minimumDuration:maximumDistance:pressing:perform:) 

Instance Method

# onLongPressGesture(minimumDuration:maximumDistance:pressing:perform:)

Adds an action to perform when this view recognizes a long press gesture.

Journaling SuggestionsSwiftUIiOS 13.0–18.4DeprecatedmacOS 10.15+visionOSwatchOS 6.0+

``` source
nonisolated
func onLongPressGesture(
    minimumDuration: Double = 0.5,
    maximumDistance: CGFloat = 10,
    pressing: ((Bool) -> Void)? = nil,
    perform action: @escaping () -> Void
) -> some View
```

