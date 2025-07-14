

- Journaling Suggestions
- JournalingSuggestionsPicker
-  fileDialogImportsUnresolvedAliases(\_:) 

Instance Method

# fileDialogImportsUnresolvedAliases(\_:)

On macOS, configures the `fileExporter`, `fileImporter`, or `fileMover` behavior when a user chooses an alias.

Journaling SuggestionsSwiftUIiOS 17.0+macOS 14.0+

``` source
nonisolated
func fileDialogImportsUnresolvedAliases(_ imports: Bool) -> some View
```

## Parameters 

`imports`  

A Boolean value that indicates if the application receives unresolved or resolved URLs when a user chooses aliases.

## Discussion

By default, file dialogs resolve aliases and provide the URL of the item referred to by the chosen alias. This modifier allows control of this behavior: pass `true` if the application doesn’t want file dialog to resolve aliases.

