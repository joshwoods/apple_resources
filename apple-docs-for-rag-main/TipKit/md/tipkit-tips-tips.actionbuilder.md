

- TipKit
- Tips
-  Tips.ActionBuilder 

Structure

# Tips.ActionBuilder

The result builder for generating a tip’s actions.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@resultBuilder
struct ActionBuilder
```

## Topics

### Type Methods

static func buildArray([[Tips.Action]]) -> [Tips.Action]

Builds a tip’s actions set from a nested array of actions.

static func buildEither(first: [Tips.Action]) -> [Tips.Action]

Builds a tip’s actions set from an if-else statement that produces an array of actions from the if-then branch.

static func buildEither(second: [Tips.Action]) -> [Tips.Action]

Builds a tip’s actions set from an if-else statement that produces an array of actions from the else branch.

static func buildExpression([Tips.Action]) -> [Tips.Action]

Builds a tip’s actions set from an array of actions.

static func buildExpression(Tips.Action) -> [Tips.Action]

Builds a tip’s actions set from a single action value.

static func buildFinalResult([Tips.Action]) -> [Tips.Action]

Builds a final set of actions that the tip’s view uses.

static func buildLimitedAvailability([Tips.Action]) -> [Tips.Action]

static func buildOptional([Tips.Action]?) -> [Tips.Action]

Builds a tip’s actions set from an if statement.

static func buildPartialBlock(accumulated: [Tips.Action], next: [Tips.Action]) -> [Tips.Action]

Builds a tip’s actions set by appending an array of actions.

static func buildPartialBlock(first: [Tips.Action]) -> [Tips.Action]

Builds a tip’s actions set from an array of actions.

## See Also

### Builders

struct OptionsBuilder

The result builder for generating a tip’s options.

struct RuleBuilder

The result builder for generating a tip’s rules.

