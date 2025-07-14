

- SwiftUI
- View
-  focused(\_:) 

Instance Method

# focused(\_:)

Modifies this view by binding its focus state to the given Boolean state value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func focused(_ condition: FocusState.Binding) -> some View
```

## Parameters 

`condition`  

The focus state to bind. When focus moves to the view, the binding sets the bound value to `true`. If a caller sets the value to `true` programmatically, then focus moves to the modified view. When focus leaves the modified view, the binding sets the value to `false`. If a caller sets the value to `false`, SwiftUI automatically dismisses focus.

## Return Value

The modified view.

## Discussion

Use this modifier to cause the view to receive focus whenever the the `condition` value is `true`. You can use this modifier to observe the focus state of a single view, or programmatically set and remove focus from the view.

In the following example, a single TextField accepts a user’s desired `username`. The text field binds its focus state to the Boolean value `usernameFieldIsFocused`. A “Submit” button’s action verifies whether the name is available. If the name is unavailable, the button sets `usernameFieldIsFocused` to `true`, which causes focus to return to the text field, so the user can enter a different name.

```
@State private var username: String = ""
@FocusState private var usernameFieldIsFocused: Bool
@State private var showUsernameTaken = false

var body: some View {
    VStack {
        TextField("Choose a username.", text: $username)
            .focused($usernameFieldIsFocused)
        if showUsernameTaken {
            Text("That username is taken. Please choose another.")
        }
        Button("Submit") {
            showUsernameTaken = false
            if !isUserNameAvailable(username: username) {
                usernameFieldIsFocused = true
                showUsernameTaken = true
            }
        }
    }
}
```

To control focus by matching a value, use the focused(_:equals:) method instead.

## See Also

### Managing focus state

func focused&lt;Value>(FocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its focus state to the given state value.

var isFocused: Bool

Returns whether the nearest focusable ancestor has focus.

struct FocusState

A property wrapper type that can read and write a value that SwiftUI updates as the placement of focus within the scene changes.

struct FocusedValue

A property wrapper for observing values from the focused view or one of its ancestors.

macro Entry()

Creates an environment values, transaction, container values, or focused values entry.

protocol FocusedValueKey

A protocol for identifier types used when publishing and observing focused values.

struct FocusedBinding

A convenience property wrapper for observing and automatically unwrapping state bindings from the focused view or one of its ancestors.

func searchFocused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given Boolean value.

func searchFocused&lt;V>(FocusState&lt;V>.Binding, equals: V) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given value.

