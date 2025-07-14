

- SwiftUI
- View
-  searchFocused(\_:equals:) 

Instance Method

# searchFocused(\_:equals:)

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func searchFocused(
    _ binding: FocusState.Binding,
    equals value: V
) -> some View where V : Hashable
```

## Parameters 

`binding`  

The state binding to register. When focus moves to the associated search field, the binding sets the bound value to the corresponding match value. If a caller sets the state value programmatically to the matching value, then focus moves to the search field. When focus leaves the search field, the binding sets the bound value to `nil`. If a caller sets the value to `nil`, SwiftUI automatically dismisses focus.

`value`  

The value to match against when determining whether the binding should change.

## Return Value

The modified view.

## Discussion

To control focus by matching a simple boolean condition, use the searchFocused(_:) modifier instead.

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

func searchFocused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given Boolean value.

