

- SwiftUI
- AnyTransition
-  opacity 

Type Property

# opacity

A transition from transparent to opaque on insertion, and from opaque to transparent on removal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let opacity: AnyTransition
```

## See Also

### Getting built-in transitions

static let identity: AnyTransition

A transition that returns the input view, unmodified, as the output view.

static func move(edge: Edge) -> AnyTransition

Returns a transition that moves the view away, towards the specified edge of the view.

static func offset(CGSize) -> AnyTransition

static func offset(x: CGFloat, y: CGFloat) -> AnyTransition

static func push(from: Edge) -> AnyTransition

Creates a transition that when added to a view will animate the view’s insertion by moving it in from the specified edge while fading it in, and animate its removal by moving it out towards the opposite edge and fading it out.

static var scale: AnyTransition

Returns a transition that scales the view.

static func scale(scale: CGFloat, anchor: UnitPoint) -> AnyTransition

Returns a transition that scales the view by the specified amount.

static var slide: AnyTransition

A transition that inserts by moving in from the leading edge, and removes by moving out towards the trailing edge.

