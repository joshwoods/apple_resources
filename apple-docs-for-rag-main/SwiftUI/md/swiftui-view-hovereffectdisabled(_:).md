

- SwiftUI
- View
-  hoverEffectDisabled(\_:) 

Instance Method

# hoverEffectDisabled(\_:)

Adds a condition that controls whether this view can display hover effects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func hoverEffectDisabled(_ disabled: Bool = true) -> some View
```

## Parameters 

`disabled`  

A Boolean value that determines whether this view can display hover effects.

## Return Value

A view that controls whether hover effects can be displayed in this view.

## Discussion

The higher views in a view hierarchy can override the value you set on this view. In the following example, the button does not display a hover effect because the outer `hoverEffectDisabled(_:)` modifier overrides the inner one:

```
HStack {
    Button("Press") {}
        .hoverEffectDisabled(false)
}
.hoverEffectDisabled(true)
```

## See Also

### Responding to hover events

func onHover(perform: (Bool) -> Void) -> some View

Adds an action to perform when the user moves the pointer over or away from the view’s frame.

func onContinuousHover(coordinateSpace:perform:)

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

func hoverEffect(_:isEnabled:)

Applies a hover effect to this view.

func defaultHoverEffect(_:)

Sets the default hover effect to use for views within this view.

var isHoverEffectEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows hover effects to be displayed.

enum HoverPhase

The current hovering state and value of the pointer.

