

- SwiftUI
- EnvironmentValues
-  isHoverEffectEnabled 

Instance Property

# isHoverEffectEnabled

A Boolean value that indicates whether the view associated with this environment allows hover effects to be displayed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
var isHoverEffectEnabled: Bool { get set }
```

## Discussion

The default value is `true`.

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

func defaultHoverEffect(_:)

Sets the default hover effect to use for views within this view.

enum HoverPhase

The current hovering state and value of the pointer.

