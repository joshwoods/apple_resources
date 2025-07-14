

- DeviceActivity
- DeviceActivityReport
-  searchFocused(\_:equals:) 

Instance Method

# searchFocused(\_:equals:)

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given value.

DeviceActivitySwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

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

To control focus by matching a simple boolean condition, use the `View/searchFocused(_:)` modifier instead.

For more information about using searchable modifiers, refer to doc:Adding-a-search-interface-to-your-app.

