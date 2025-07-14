

- SwiftUI
- CommandsBuilder
-  buildLimitedAvailability(\_:) 

Type Method

# buildLimitedAvailability(\_:)

Processes commands for a conditional compiler-control statement that performs an availability check.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+visionOS 1.0+

``` source
static func buildLimitedAvailability(_ content: any Commands) -> some Commands
```

Show all declarations

## See Also

### Building conditionally

static func buildEither&lt;T, F>(first: T) -> _ConditionalContent&lt;T, F>

Produces content for a conditional statement in a multi-statement closure when the condition is true.

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

Produces content for a conditional statement in a multi-statement closure when the condition is false.

static func buildIf&lt;C>(C?) -> C?

Produces an optional widget for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

