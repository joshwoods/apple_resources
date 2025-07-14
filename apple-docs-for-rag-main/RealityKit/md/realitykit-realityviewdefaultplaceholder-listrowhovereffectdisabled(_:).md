

- RealityKit
- RealityViewDefaultPlaceholder
-  listRowHoverEffectDisabled(\_:) 

Instance Method

# listRowHoverEffectDisabled(\_:)

Requests that the containing list row have its hover effect disabled.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
func listRowHoverEffectDisabled(_ disabled: Bool = true) -> some View
```

## Parameters 

`disabled`  

A Boolean value that determines whether the containing list row should display its default hover effect.

## Return Value

A view that requests the default hover effect on its containing list row to conditionally be disabled.

## Discussion

By default, `List` rows have built-in hover effects in visionOS. In some cases, it is useful to disable the default hover effect.

