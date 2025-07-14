

- SwiftUI
- View
-  focusScope(\_:) 

Instance Method

# focusScope(\_:)

Creates a focus scope that SwiftUI uses to limit default focus preferences.

macOS 12.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func focusScope(_ namespace: Namespace.ID) -> some View
```

## Parameters 

`namespace`  

A namespace identifier that SwiftUI can use to scope default focus preferences.

## Return Value

A view that sets the namespace of descendants for default focus.

## Discussion

The returned view gets associated with the provided namespace. Pass this namespace to prefersDefaultFocus(_:in:) and the resetFocus function.

## See Also

### Setting focus scope

func focusSection() -> some View

Indicates that the view’s frame and cohort of focusable descendants should be used to guide focus movement.

