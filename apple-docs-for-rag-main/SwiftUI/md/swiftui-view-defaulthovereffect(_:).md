

- SwiftUI
- View
-  defaultHoverEffect(\_:) 

Instance Method

# defaultHoverEffect(\_:)

Sets the default hover effect to use for views within this view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func defaultHoverEffect(_ effect: HoverEffect?) -> some View
```

Show all declarations

## Parameters 

`effect`  

The default hover effect to use for views within this view.

## Return Value

A view that uses this effect as the default hover effect.

## Discussion

Use this modifier to set a specific hover effect for all views with the hoverEffect(_:) modifier applied within a view. The default effect is typically used when no HoverEffect was provided or if automatic is specified.

For example, this view uses highlight for both the red and green Color views:

```
HStack {
    Color.red.hoverEffect()
    Color.green.hoverEffect()
}
.defaultHoverEffect(.highlight)
```

This also works for customizing the default hover effect in views like Buttons when using a SwiftUI-defined style like `ButtonStyle/bordered`, which can provide a hover effect by default. For example, this view replaces the hover effect for a Button with highlight:

```
Button("Next") {}
    // perform action
}
.buttonStyle(.bordered)
.defaultHoverEffect(.highlight)
```

Use a `nil` effect to indicate that the default hover effect should not be modified.

## See Also

### Responding to hover events

func onHover(perform: (Bool) -> Void) -> some View

Adds an action to perform when the user moves the pointer over or away from the view’s frame.

func onContinuousHover(coordinateSpace:perform:)

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

func hoverEffect(_:isEnabled:)

Applies a hover effect to this view.

func hoverEffectDisabled(Bool) -> some View

Adds a condition that controls whether this view can display hover effects.

var isHoverEffectEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows hover effects to be displayed.

enum HoverPhase

The current hovering state and value of the pointer.

