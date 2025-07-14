

- SwiftUI
-  HoverPhase 

Enumeration

# HoverPhase

The current hovering state and value of the pointer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@frozen
enum HoverPhase
```

## Overview

When you use the onContinuousHover(coordinateSpace:perform:) modifier, you can handle the hovering state using the `action` closure. SwiftUI calls the closure with a phase value to indicate the current hovering state. The following example updates `hoverLocation` and `isHovering` based on the phase provided to the closure:

```
@State private var hoverLocation: CGPoint = .zero
@State private var isHovering = false

var body: some View {
    VStack {
        Color.red
            .frame(width: 400, height: 400)
            .onContinuousHover { phase in
                switch phase {
                case .active(let location):
                    hoverLocation = location
                    isHovering = true
                case .ended:
                    isHovering = false
                }
            }
            .overlay {
                Rectangle()
                    .frame(width: 50, height: 50)
                    .foregroundColor(isHovering ? .green : .blue)
                    .offset(x: hoverLocation.x, y: hoverLocation.y)
            }
    }
}
```

## Topics

### Getting hover phases

case active(CGPoint)

The pointer’s location moved to the specified point within the view.

case ended

The pointer exited the view.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Sendable

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

var isHoverEffectEnabled: Bool

A Boolean value that indicates whether the view associated with this environment allows hover effects to be displayed.

