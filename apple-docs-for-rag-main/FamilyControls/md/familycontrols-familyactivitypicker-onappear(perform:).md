

- FamilyControls
- FamilyActivityPicker
-  onAppear(perform:) 

Instance Method

# onAppear(perform:)

Adds an action to perform before this view appears.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func onAppear(perform action: (() -> Void)? = nil) -> some View
```

## Parameters 

`action`  

The action to perform. If `action` is `nil`, the call has no effect.

## Return Value

A view that triggers `action` before it appears.

## Discussion

The exact moment that SwiftUI calls this method depends on the specific view type that you apply it to, but the `action` closure completes before the first rendered frame appears.

## See Also

### View Life Cycle

func onDisappear(perform: (() -> Void)?) -> some View

Adds an action to perform after this view disappears.

func onChange&lt;V>(of: V, perform: (V) -> Void) -> some View

Performs an action when a specified value changes.

Deprecated

