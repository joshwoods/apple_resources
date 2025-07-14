

- Journaling Suggestions
- JournalingSuggestionsPicker
-  init(\_:onCompletion:) 

Initializer

# init(\_:onCompletion:)

Creates a suggestions picker with button text defined by the given string.

iOS 17.2+

``` source
@MainActor @preconcurrency
init(
    _ title: S,
    onCompletion: @escaping (JournalingSuggestion) async -> Void
) where S : StringProtocol
```

Available when `Label` is `Text`.

## Parameters 

`title`  

A string that describes the suggestion picker’s purpose in the context of your app.

`onCompletion`  

Code that you supply, which processes any suggestions that a person chooses in the picker.

## Discussion

This initializer creates a text view on your behalf and uses the string argument to set its text.

## See Also

### Creating a suggestions picker

init(label: () -> Label, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker within the given view.

init(LocalizedStringKey, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker with button text defined by the given localized string key.

