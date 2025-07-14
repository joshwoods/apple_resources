

- SwiftUI
- View
-  focusable(\_:) 

Instance Method

# focusable(\_:)

Specifies if the view is focusable.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

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

### Indicating that a view can receive focus

func focusable(Bool, interactions: FocusInteractions) -> some View

Specifies if the view is focusable, and if so, what focus-driven interactions it supports.

struct FocusInteractions

Values describe different focus interactions that a view can support.

