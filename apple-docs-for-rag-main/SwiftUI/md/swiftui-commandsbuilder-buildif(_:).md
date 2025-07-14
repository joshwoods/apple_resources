

- SwiftUI
- CommandsBuilder
-  buildIf(\_:) 

Type Method

# buildIf(\_:)

Produces an optional widget for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
static func buildIf(_ content: C?) -> C? where C : Commands
```

## See Also

### Building conditionally

static func buildEither&lt;T, F>(first: T) -> _ConditionalContent&lt;T, F>

Produces content for a conditional statement in a multi-statement closure when the condition is true.

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

Produces content for a conditional statement in a multi-statement closure when the condition is false.

static buildLimitedAvailability(_:)

Processes commands for a conditional compiler-control statement that performs an availability check.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

