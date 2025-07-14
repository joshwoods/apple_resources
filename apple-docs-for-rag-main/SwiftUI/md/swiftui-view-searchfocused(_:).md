

- SwiftUI
- View
-  searchFocused(\_:) 

Instance Method

# searchFocused(\_:)

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given Boolean value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func searchFocused(_ binding: FocusState.Binding) -> some View
```

## Return Value

The modified view.

## Discussion

To control focus by matching a non-boolean value, use the searchFocused(_:equals:) modifier instead.

For more information about using searchable modifiers, refer to Adding a search interface to your app.

## See Also

### Managing focus state

func focused&lt;Value>(FocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its focus state to the given state value.

func focused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding its focus state to the given Boolean state value.

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

func searchFocused&lt;V>(FocusState&lt;V>.Binding, equals: V) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given value.

