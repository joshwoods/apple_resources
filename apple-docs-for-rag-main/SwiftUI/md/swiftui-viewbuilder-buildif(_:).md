

- SwiftUI
- ViewBuilder
-  buildIf(\_:) 

Type Method

# buildIf(\_:)

Produces an optional view for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func buildIf(_ content: Content?) -> Content? where Content : View
```

## See Also

### Conditionally building content

static func buildEither&lt;TrueContent, FalseContent>(first: TrueContent) -> _ConditionalContent&lt;TrueContent, FalseContent>

Produces content for a conditional statement in a multi-statement closure when the condition is true.

static func buildEither&lt;TrueContent, FalseContent>(second: FalseContent) -> _ConditionalContent&lt;TrueContent, FalseContent>

Produces content for a conditional statement in a multi-statement closure when the condition is false.

static func buildLimitedAvailability&lt;Content>(Content) -> AnyView

Processes view content for a conditional compiler-control statement that performs an availability check.

