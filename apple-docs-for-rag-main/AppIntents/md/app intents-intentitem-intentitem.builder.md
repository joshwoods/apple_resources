

- App Intents
- IntentItem
-  IntentItem.Builder 

Enumeration

# IntentItem.Builder

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum Builder
```

Available when `Value` conforms to `_IntentValue`.

## Topics

### Type Methods

static func buildArray([[IntentItem&lt;Value>]]) -> [IntentItem&lt;Value>]

static func buildBlock() -> [Value]

static func buildBlock(IntentItem&lt;Value>...) -> [IntentItem&lt;Value>]

static func buildBlock([IntentItem&lt;Value>]) -> [IntentItem&lt;Value>]

static func buildExpression(Value) -> IntentItem&lt;Value>

static func buildExpression&lt;ExpressionValue>(IntentItem&lt;ExpressionValue>) -> IntentItem&lt;ExpressionValue>

