

- MapKit
- MapContentBuilder
-  buildIf(\_:) 

Type Method

# buildIf(\_:)

Compares content in a multistatement closure, that produces an optional view that’s visible if the argument you provide evaluates to true.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func buildIf(_ content: Content?) -> Content? where Content : MapContent
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

static func buildLimitedAvailability(any MapContent) -> some MapContent

Provides support for “if” statements with “available” macro clauses in multi-statement closures, producing conditional content for the “then” branch, such the conditionally-available branch.

