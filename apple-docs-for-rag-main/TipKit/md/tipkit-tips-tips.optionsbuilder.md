

- TipKit
- Tips
-  Tips.OptionsBuilder 

Structure

# Tips.OptionsBuilder

The result builder for generating a tip’s options.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@resultBuilder
struct OptionsBuilder
```

## Topics

### Type Methods

static func buildBlock() -> some TipOption

static func buildEither(first: some TipOption) -> some TipOption

static func buildEither(second: some TipOption) -> some TipOption

static func buildExpression((any TipOption)?) -> some TipOption

static func buildExpression([some TipOption]) -> some TipOption

static func buildExpression(some TipOption) -> some TipOption

static func buildExpression([(any TipOption)?]) -> some TipOption

static func buildFinalResult(some TipOption) -> [any TipOption]

static func buildOptional([(any TipOption)?]) -> some TipOption

static func buildOptional((any TipOption)?) -> some TipOption

static func buildPartialBlock(accumulated: some TipOption, next: some TipOption) -> some TipOption

static func buildPartialBlock(first: some TipOption) -> some TipOption

## See Also

### Builders

struct ActionBuilder

The result builder for generating a tip’s actions.

struct RuleBuilder

The result builder for generating a tip’s rules.

