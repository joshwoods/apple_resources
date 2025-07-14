

- Swift Charts
-  AxisContentBuilder 

Structure

# AxisContentBuilder

A result builder that constructs axis content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
struct AxisContentBuilder
```

## Topics

### Type Methods

static func buildBlock() -> some AxisContent

static func buildBlock&lt;T>(T) -> T

Builds a result from a single component.

static func buildBlock&lt;each T>(repeat each T) -> some AxisContent

Builds a result from multiple components.

static func buildEither&lt;T1, T2>(first: T1) -> BuilderConditional&lt;T1, T2>

Provides support for “if-else” statements in multi-statement closures, producing conditional content for the “then” branch.

static func buildEither&lt;T1, T2>(second: T2) -> BuilderConditional&lt;T1, T2>

Provides support for “if-else” statements in multi-statement closures, producing conditional content for the “else” branch.

static func buildExpression&lt;Content>(Content) -> Content

static func buildIf&lt;T>(T?) -> T?

Provides support for “if” statements in multi-statement closures, producing an optional axis content that is visible only when the condition evaluates to `true`.

static func buildLimitedAvailability&lt;Content>(Content) -> AnyAxisContent

Provides support for “if” statements with `#available()` clauses in multi-statement closures, producing conditional content for the “then” branch, i.e. the conditionally-available branch.

static func buildPartialBlock(accumulated: some AxisContent, next: some AxisContent) -> some AxisContentDeprecated

static func buildPartialBlock&lt;T>(first: T) -> TDeprecated

## See Also

### Axes

Customizing axes in Swift Charts

Improve the clarity of your chart by configuring the appearance of its axes.

struct ChartAxisContent

A view that represents a chart’s axis.

protocol AxisContent

A type that represents the elements you use to build a chart’s axes.

struct AxisMarks

A group of visual marks that a chart draws to indicate the composition of a chart’s axes.

struct AnyAxisContent

A type-erased element of a chart’s axis.

