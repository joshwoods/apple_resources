

- DeviceActivity
- DeviceActivityReport
-  accessibilityFocused(\_:equals:) 

Instance Method

# accessibilityFocused(\_:equals:)

Modifies this view by binding its accessibility element’s focus state to the given state value.

DeviceActivitySwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func accessibilityFocused(
    _ binding: AccessibilityFocusState.Binding,
    equals value: Value
) -> some View where Value : Hashable
```

## Parameters 

`binding`  

The state binding to register. When accessibility focus moves to the accessibility element of the modified view, SwiftUI sets the bound value to the corresponding match value. If you set the state value programmatically to the matching value, then accessibility focus moves to the accessibility element of the modified view. SwiftUI sets the value to `nil` if accessibility focus leaves the accessibility element associated with the modified view, and programmatically setting the value to `nil` dismisses focus automatically.

`value`  

The value to match against when determining whether the binding should change.

## Return Value

The modified view.

