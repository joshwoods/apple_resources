

- Swift Charts
- ChartContentBuilder
-  buildIf(\_:) 

Type Method

# buildIf(\_:)

Builds a partial result that’s conditionally present.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildIf(_ content: T?) -> T? where T : ChartContent
```

## Parameters 

`content`  

The content to use if the condition is `true`.

## Discussion

This method provides support for `if` statements. It produces optional chart content that is visible only when the condition evaluates to `true`.

## See Also

### Building conditionally

static func buildEither&lt;T1, T2>(first: T1) -> BuilderConditional&lt;T1, T2>

Builds a partial result from a condition that’s true.

static func buildEither&lt;T1, T2>(second: T2) -> BuilderConditional&lt;T1, T2>

Builds a partial result from a condition that’s false.

