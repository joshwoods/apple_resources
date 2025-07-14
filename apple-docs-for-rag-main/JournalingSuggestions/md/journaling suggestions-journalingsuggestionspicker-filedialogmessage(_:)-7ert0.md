

- Journaling Suggestions
- JournalingSuggestionsPicker
-  fileDialogMessage(\_:) 

Instance Method

# fileDialogMessage(\_:)

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom message that is presented to the user, similar to a title.

Journaling SuggestionsSwiftUIiOS 17.0+macOS 14.0+

``` source
nonisolated
func fileDialogMessage(_ message: S) -> some View where S : StringProtocol
```

## Parameters 

`message`  

The string to use as the file dialog message.

