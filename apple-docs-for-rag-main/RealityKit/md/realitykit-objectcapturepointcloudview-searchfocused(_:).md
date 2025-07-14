

- RealityKit
- ObjectCapturePointCloudView
-  searchFocused(\_:) 

Instance Method

# searchFocused(\_:)

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given Boolean value.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func searchFocused(_ binding: FocusState.Binding) -> some View
```

## Parameters 

`condition`  

The focus state to bind. When focus moves to the associated search field, the binding sets the bound value to `true`. If a caller sets the value to `true` programmatically, then focus moves to the search field. When focus leaves the search field, the binding sets the value to `false`. If a caller sets the value to `false`, SwiftUI automatically dismisses focus.

## Return Value

The modified view.

## Discussion

To control focus by matching a non-boolean value, use the `View/searchFocused(_:equals:)` modifier instead.

For more information about using searchable modifiers, refer to doc:Adding-a-search-interface-to-your-app.

