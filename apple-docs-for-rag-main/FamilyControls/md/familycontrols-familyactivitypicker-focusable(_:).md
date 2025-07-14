

- FamilyControls
- FamilyActivityPicker
-  focusable(\_:) 

Instance Method

# focusable(\_:)

Specifies if the view is focusable.

FamilyControlsSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func focusable(_ isFocusable: Bool = true) -> some View
```

## Parameters 

`isFocusable`  

A Boolean value that indicates whether this view is focusable.

## Return Value

A view that sets whether a view is focusable.

## See Also

### Focus

func focused&lt;Value>(FocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its focus state to the given state value.

func focused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding its focus state to the given Boolean state value.

