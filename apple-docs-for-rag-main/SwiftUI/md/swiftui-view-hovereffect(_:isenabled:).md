

- SwiftUI
- View
-  hoverEffect(\_:isEnabled:) 

Instance Method

# hoverEffect(\_:isEnabled:)

Applies a hover effect to this view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func hoverEffect(
    _ effect: HoverEffect = .automatic,
    isEnabled: Bool = true
) -> some View
```

Show all declarations

## Parameters 

`effect`  

The effect to apply to this view.

`isEnabled`  

Whether the effect is enabled or not.

## Return Value

A new view that applies a hover effect to `self`.

## Discussion

By default, automatic is used. You can control the behavior of the automatic effect with the defaultHoverEffect(_:) modifier.

## See Also

### Responding to hover events

func onHover(perform: (Bool) -> Void) -> some View

Adds an action to perform when the user moves the pointer over or away from the view’s frame.

func onContinuousHover(coordinateSpace:perform:)

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

func hoverEffectDisabled(Bool) -> some View

Adds a condition that controls whether this view can display hover effects.

func defaultHoverEffect(_:)

Sets the default hover effect to use for views within this view.

var isHoverEffectEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows hover effects to be displayed.

enum HoverPhase

The current hovering state and value of the pointer.

