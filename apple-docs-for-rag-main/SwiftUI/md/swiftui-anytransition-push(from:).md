

- SwiftUI
- AnyTransition
-  push(from:) 

Type Method

# push(from:)

Creates a transition that when added to a view will animate the view’s insertion by moving it in from the specified edge while fading it in, and animate its removal by moving it out towards the opposite edge and fading it out.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func push(from edge: Edge) -> AnyTransition
```

## Parameters 

`edge`  

The edge from which the view will be animated in.

## Return Value

A transition that animates a view by moving and fading it.

## See Also

### Getting built-in transitions

static let identity: AnyTransition

A transition that returns the input view, unmodified, as the output view.

static func move(edge: Edge) -> AnyTransition

Returns a transition that moves the view away, towards the specified edge of the view.

static func offset(CGSize) -> AnyTransition

static func offset(x: CGFloat, y: CGFloat) -> AnyTransition

static let opacity: AnyTransition

A transition from transparent to opaque on insertion, and from opaque to transparent on removal.

static var scale: AnyTransition

Returns a transition that scales the view.

static func scale(scale: CGFloat, anchor: UnitPoint) -> AnyTransition

Returns a transition that scales the view by the specified amount.

static var slide: AnyTransition

A transition that inserts by moving in from the leading edge, and removes by moving out towards the trailing edge.

