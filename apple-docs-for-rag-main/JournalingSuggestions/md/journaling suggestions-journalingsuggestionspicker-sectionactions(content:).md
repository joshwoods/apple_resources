

- Journaling Suggestions
- JournalingSuggestionsPicker
-  sectionActions(content:) 

Instance Method

# sectionActions(content:)

Adds custom actions to a section.

Journaling SuggestionsSwiftUIiOS 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func sectionActions(@ViewBuilder content: () -> Content) -> some View where Content : View
```

## Discussion

On iOS, the actions are displayed as items after the content of the section. On macOS, the actions are displayed when a user hovers over the section.

The following example adds an ‘Add’ button to the ‘Categories’ section.

```
List {
    Label("Home", systemImage: "house")
    Label("Alerts", systemImage: "bell")

    Section("Categories") {
        Label("Climate", systemImage: "fan")
        Label("Lights", systemImage: "lightbulb")
    }
    .sectionActions {
        Button("Add Category", systemImage: "plus") { }
    }
}
```

