

- SwiftUI
- SceneBuilder
-  buildExpression(\_:) 

Type Method

# buildExpression(\_:)

Builds an expression within the builder.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func buildExpression(_ content: Content) -> Content where Content : Scene
```

## See Also

### Building content

static buildBlock(_:)

Passes a single scene written as a child scene through unmodified.

static buildLimitedAvailability(_:)

Processes scene content for a conditional compiler-control statement that performs an availability check.

static func buildOptional((any Scene &amp; _LimitedAvailabilitySceneMarker)?) -> some Scene

Produces an optional scene for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

