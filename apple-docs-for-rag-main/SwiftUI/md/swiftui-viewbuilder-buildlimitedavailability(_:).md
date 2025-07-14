

- SwiftUI
- ViewBuilder
-  buildLimitedAvailability(\_:) 

Type Method

# buildLimitedAvailability(\_:)

Processes view content for a conditional compiler-control statement that performs an availability check.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func buildLimitedAvailability(_ content: Content) -> AnyView where Content : View
```

## See Also

### Conditionally building content

static func buildEither&lt;TrueContent, FalseContent>(first: TrueContent) -> _ConditionalContent&lt;TrueContent, FalseContent>

Produces content for a conditional statement in a multi-statement closure when the condition is true.

static func buildEither&lt;TrueContent, FalseContent>(second: FalseContent) -> _ConditionalContent&lt;TrueContent, FalseContent>

Produces content for a conditional statement in a multi-statement closure when the condition is false.

static func buildIf&lt;Content>(Content?) -> Content?

Produces an optional view for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

