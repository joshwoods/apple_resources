

- SwiftUI
- CommandsBuilder
-  buildExpression(\_:) 

Type Method

# buildExpression(\_:)

Builds an expression within the builder.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static func buildExpression(_ content: Content) -> Content where Content : Commands
```

## See Also

### Building conditionally

static func buildEither&lt;T, F>(first: T) -> _ConditionalContent&lt;T, F>

Produces content for a conditional statement in a multi-statement closure when the condition is true.

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

Produces content for a conditional statement in a multi-statement closure when the condition is false.

static func buildIf&lt;C>(C?) -> C?

Produces an optional widget for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

static buildLimitedAvailability(_:)

Processes commands for a conditional compiler-control statement that performs an availability check.

