

- TipKit
- Tips
-  Tips.RuleBuilder 

Structure

# Tips.RuleBuilder

The result builder for generating a tip’s rules.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@resultBuilder
struct RuleBuilder
```

## Topics

### Type Methods

static func buildBlock() -> [Tips.Rule]

static func buildEither(first: [Tips.Rule]) -> [Tips.Rule]

static func buildEither(second: [Tips.Rule]) -> [Tips.Rule]

static func buildExpression(Tips.Rule?) -> [Tips.Rule]

static func buildExpression([Tips.Rule]) -> [Tips.Rule]

static func buildExpression(Tips.Rule) -> [Tips.Rule]

static func buildExpression([Tips.Rule?]) -> [Tips.Rule]

static func buildOptional(Tips.Rule?) -> [Tips.Rule]

static func buildOptional([Tips.Rule?]) -> [Tips.Rule]

static func buildPartialBlock(accumulated: [Tips.Rule], next: [Tips.Rule]) -> [Tips.Rule]

static func buildPartialBlock(first: [Tips.Rule]) -> [Tips.Rule]

## See Also

### Builders

struct ActionBuilder

The result builder for generating a tip’s actions.

struct OptionsBuilder

The result builder for generating a tip’s options.

