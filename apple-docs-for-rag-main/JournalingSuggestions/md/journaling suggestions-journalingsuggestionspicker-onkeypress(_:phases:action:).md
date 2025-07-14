

- Journaling Suggestions
- JournalingSuggestionsPicker
-  onKeyPress(\_:phases:action:) 

Instance Method

# onKeyPress(\_:phases:action:)

Performs an action if the user presses a key on a hardware keyboard while the view has focus.

Journaling SuggestionsSwiftUIiOS 17.0+macOS 14.0+tvOS 17.0+

``` source
nonisolated
func onKeyPress(
    _ key: KeyEquivalent,
    phases: KeyPress.Phases,
    action: @escaping (KeyPress) -> KeyPress.Result
) -> some View
```

## Parameters 

`key`  

The key to match against incoming hardware keyboard events.

`phases`  

The key-press phases to match (`.down`, `.up`, and `.repeat`).

`action`  

The action to perform. The action receives a value describing the matched key event. Return `.handled` to consume the event and prevent further dispatch, or `.ignored` to allow dispatch to continue.

## Return Value

A modified view that binds hardware keyboard input when focused.

## Discussion

SwiftUI performs the action for the specified event phases.

