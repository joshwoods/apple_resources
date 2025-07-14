

- Journaling Suggestions
- JournalingSuggestionsPicker
-  init(\_:onCompletion:) 

Initializer

# init(\_:onCompletion:)

Creates a suggestions picker with button text defined by the given localized string key.

iOS 17.2+

``` source
@MainActor @preconcurrency
init(
    _ title: LocalizedStringKey,
    onCompletion: @escaping (JournalingSuggestion) async -> Void
)
```

Available when `Label` is `Text`.

## Parameters 

`title`  

A localized string key that describes the suggestion picker’s purpose in the context of your app.

`onCompletion`  

Code that you supply, which processes any suggestions that a person chooses in the picker.

## Discussion

This initializer creates a text view similar to the results of calling init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

## See Also

### Creating a suggestions picker

init(label: () -> Label, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker within the given view.

init&lt;S>(S, onCompletion: (JournalingSuggestion) async -> Void)

Creates a suggestions picker with button text defined by the given string.

