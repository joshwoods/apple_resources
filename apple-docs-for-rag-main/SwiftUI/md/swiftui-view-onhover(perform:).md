

- SwiftUI
- View
-  onHover(perform:) 

Instance Method

# onHover(perform:)

Adds an action to perform when the user moves the pointer over or away from the view’s frame.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+visionOS 1.0+

``` source
nonisolated
func onHover(perform action: @escaping (Bool) -> Void) -> some View
```

## Parameters 

`action`  

The action to perform whenever the pointer enters or exits this view’s frame. If the pointer is in the view’s frame, the `action` closure passes `true` as a parameter; otherwise, `false`.

## Return Value

A view that triggers `action` when the pointer enters or exits this view’s frame.

## Discussion

Calling this method defines a region for detecting pointer movement with the size and position of this view.

## See Also

### Responding to hover events

func onContinuousHover(coordinateSpace:perform:)

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

func hoverEffect(_:isEnabled:)

Applies a hover effect to this view.

func hoverEffectDisabled(Bool) -> some View

Adds a condition that controls whether this view can display hover effects.

func defaultHoverEffect(_:)

Sets the default hover effect to use for views within this view.

var isHoverEffectEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows hover effects to be displayed.

enum HoverPhase

The current hovering state and value of the pointer.

