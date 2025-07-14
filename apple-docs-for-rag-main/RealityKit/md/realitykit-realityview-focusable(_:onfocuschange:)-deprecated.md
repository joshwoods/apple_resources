

- RealityKit
- RealityView
-  focusable(\_:onFocusChange:) Deprecated

Instance Method

# focusable(\_:onFocusChange:)

Specifies if the view is focusable and, if so, adds an action to perform when the view comes into focus.

RealityKitSwiftUImacOS 10.15–12.0DeprecatedtvOS 13.0–15.0DeprecatedwatchOS 6.0–8.0Deprecated

``` source
nonisolated
func focusable(
    _ isFocusable: Bool = true,
    onFocusChange: @escaping (Bool) -> Void = { _ in }
) -> some View
```

Deprecated

Use FocusState\ and View.focused(\_:equals) for functionality previously provided by the onChange parameter.

## Parameters 

`isFocusable`  

A Boolean value that indicates whether this view is focusable.

`onFocusChange`  

A closure that’s called whenever this view either gains or loses focus. The Boolean parameter to `onFocusChange` is `true` when the view is in focus; otherwise, it’s `false`.

## Return Value

A view that sets whether a view is focusable, and triggers `onFocusChange` when the view gains or loses focus.

