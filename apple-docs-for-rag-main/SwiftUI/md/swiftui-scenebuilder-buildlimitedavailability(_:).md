

- SwiftUI
- SceneBuilder
-  buildLimitedAvailability(\_:) 

Type Method

# buildLimitedAvailability(\_:)

Processes scene content for a conditional compiler-control statement that performs an availability check.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
static func buildLimitedAvailability(_ scene: some Scene) -> any Scene & _LimitedAvailabilitySceneMarker
```

Show all declarations

## See Also

### Building content

static buildBlock(_:)

Passes a single scene written as a child scene through unmodified.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

static func buildOptional((any Scene &amp; _LimitedAvailabilitySceneMarker)?) -> some Scene

Produces an optional scene for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

