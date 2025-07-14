

- Journaling Suggestions
- JournalingSuggestionsPicker
-  buttonStyle(\_:) 

Instance Method

# buttonStyle(\_:)

Sets the style for buttons within this view to a button style with a custom appearance and custom interaction behavior.

Journaling SuggestionsSwiftUIiOS 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func buttonStyle(_ style: S) -> some View where S : PrimitiveButtonStyle
```

## Discussion

Use this modifier to set a specific style for button instances within a view:

```
HStack {
    Button("Sign In", action: signIn)
    Button("Register", action: register)
}
.buttonStyle(.bordered)
```

