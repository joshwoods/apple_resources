

- MapKit
- MapContentBuilder
-  buildLimitedAvailability(\_:) 

Type Method

# buildLimitedAvailability(\_:)

Provides support for “if” statements with “available” macro clauses in multi-statement closures, producing conditional content for the “then” branch, such the conditionally-available branch.

MapKitSwiftUIiOS 17.5+iPadOS 17.5+Mac CatalystmacOS 14.5+tvOS 17.5+visionOS 1.2+watchOS 10.5+

``` source
static func buildLimitedAvailability(_ content: any MapContent) -> some MapContent
```

## Parameters 

`content`  

The map builder content the expression builder operates on.

## Return Value

Returns the conditional map content that meets the conditions the content builder expresses.

## See Also

### Conditionally building map content

static func buildEither&lt;TrueContent, FalseContent>(first: TrueContent) -> _ConditionalMapContent&lt;TrueContent, FalseContent>

Compares content in a multistatement closure, resulting in use of the conditional content if the first argument you provide evaluates to  true.

static func buildEither&lt;TrueContent, FalseContent>(second: FalseContent) -> _ConditionalMapContent&lt;TrueContent, FalseContent>

Compares content in a multistatement closure, resulting in use of the conditional content if the second argument you provide evaluates to true.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the map content builder.

static func buildIf&lt;Content>(Content?) -> Content?

Compares content in a multistatement closure, that produces an optional view that’s visible if the argument you provide evaluates to true.

