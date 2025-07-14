

- Journaling Suggestions
- JournalingSuggestionsPicker
-  journalingSuggestionsPicker(isPresented:onCompletion:) 

Instance Method

# journalingSuggestionsPicker(isPresented:onCompletion:)

Presents a visual picker interface that contains events and images that a person can select to retrieve more information.

Journaling SuggestionsSwiftUIiOS 17.2+

``` source
@MainActor @preconcurrency
func journalingSuggestionsPicker(
    isPresented: Binding,
    onCompletion: @escaping (JournalingSuggestion) async -> Void
) -> some View
```

## Parameters 

`isPresented`  

A binding to a `Bool` value that determines whether to show the picker.

`onCompletion`  

Code that you supply, which processes any suggestions that a person may choose in the picker.

## Discussion

For more information about the Journaling Suggestions picker, see: Presenting the suggestions picker and processing a selection.

