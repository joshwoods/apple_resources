

- Swift Charts
- ChartContentBuilder
-  buildEither(second:) 

Type Method

# buildEither(second:)

Builds a partial result from a condition that’s false.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildEither(second: T2) -> BuilderConditional where T1 : ChartContent, T2 : ChartContent
```

## Parameters 

`second`  

The content to use if the condition is `false`.

## Discussion

This method provides support for `if` statements with an `else` clause and `switch` statements. It produces optional chart content that is visible when the condition evaluates to `false`.

## See Also

### Building conditionally

static func buildIf&lt;T>(T?) -> T?

Builds a partial result that’s conditionally present.

static func buildEither&lt;T1, T2>(first: T1) -> BuilderConditional&lt;T1, T2>

Builds a partial result from a condition that’s true.

