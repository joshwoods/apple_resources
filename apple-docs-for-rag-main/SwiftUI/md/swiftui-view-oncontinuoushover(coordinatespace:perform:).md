

- SwiftUI
- View
-  onContinuousHover(coordinateSpace:perform:) 

Instance Method

# onContinuousHover(coordinateSpace:perform:)

Adds an action to perform when the pointer enters, moves within, and exits the view’s bounds.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func onContinuousHover(
    coordinateSpace: some CoordinateSpaceProtocol = .local,
    perform action: @escaping (HoverPhase) -> Void
) -> some View
```

Show all declarations

## Parameters 

`coordinateSpace`  

The coordinate space for the location values. The default value is CoordinateSpace.local.

`action`  

The action to perform whenever the pointer enters, moves within, or exits the view’s bounds. The closure takes a `phase` input that has the value HoverPhase.active(_:) and contains the pointer’s coordinates if the pointer is within the view’s bounds. The closure receives the HoverPhase.ended phase when the pointer leaves the view’s bounds.

## Return Value

A view that calls `action` when the pointer enters, moves within, or exits the view’s bounds.

## Discussion

Use this modifier to define a region for detecting pointer movement with a view. The following example updates a small rectangle’s position and style by modifying `hoverLocation` and `isHovering` as the pointer moves within the larger, red rectangle:

```
@State private var hoverLocation: CGPoint = .zero
@State private var isHovering = false

var body: some View {
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
                .foregroundStyle(isHovering ? .green : .blue)
                .offset(x: hoverLocation.x, y: hoverLocation.y)
        }
}
```

## See Also

### Responding to hover events

func onHover(perform: (Bool) -> Void) -> some View

Adds an action to perform when the user moves the pointer over or away from the view’s frame.

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

