

- Journaling Suggestions
- JournalingSuggestionsPicker
-  accessibilityValue(\_:isEnabled:) 

Instance Method

# accessibilityValue(\_:isEnabled:)

Adds a textual description of the value that the view contains.

Journaling SuggestionsSwiftUIiOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityValue(
    _ value: S,
    isEnabled: Bool
) -> ModifiedContent where S : StringProtocol
```

## Parameters 

`value`  

The accessibility value to apply.

`isEnabled`  

If true the accessibility value is applied; otherwise the accessibility value is unchanged.

## Discussion

Use this method to describe the value represented by a view, but only if that’s different than the view’s label. For example, for a slider that you label as “Volume” using accessibilityLabel(), you can provide the current volume setting, like “60%”, using accessibilityValue().

