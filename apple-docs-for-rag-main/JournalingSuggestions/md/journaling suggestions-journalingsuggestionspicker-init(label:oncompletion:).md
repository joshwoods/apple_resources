

- Journaling Suggestions
- JournalingSuggestionsPicker
-  init(label:onCompletion:) 

Initializer

# init(label:onCompletion:)

Creates a suggestions picker within the given view.

iOS 17.2+

``` source
@MainActor @preconcurrency
init(
    @ViewBuilder label: () -> Label,
    onCompletion: @escaping (JournalingSuggestion) async -> Void
)
```

## Parameters 

`label`  

A view that describes the suggestion picker’s purpose in the context of your app.

`onCompletion`  

Code that you supply, which processes any suggestions that a person chooses in the picker.

## See Also

### Creating a suggestions picker

init(LocalizedStringKey, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker with button text defined by the given localized string key.

init&lt;S>(S, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker with button text defined by the given string.

