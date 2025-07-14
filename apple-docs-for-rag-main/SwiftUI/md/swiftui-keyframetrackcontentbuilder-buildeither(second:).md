

- SwiftUI
- KeyframeTrackContentBuilder
-  buildEither(second:) 

Type Method

# buildEither(second:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func buildEither(second component: Second) -> KeyframeTrackContentBuilder.Conditional where Value == First.Value, First : KeyframeTrackContent, Second : KeyframeTrackContent, First.Value == Second.Value
```

## See Also

### Building keyframe track content

static func buildArray([some KeyframeTrackContent&lt;Value>]) -> some KeyframeTrackContent&lt;Value> 

static func buildBlock() -> some KeyframeTrackContent&lt;Value> 

static func buildEither&lt;First, Second>(first: First) -> KeyframeTrackContentBuilder&lt;Value>.Conditional&lt;Value, First, Second>

static func buildExpression&lt;K>(K) -> K

static func buildPartialBlock(accumulated: some KeyframeTrackContent&lt;Value>, next: some KeyframeTrackContent&lt;Value>) -> some KeyframeTrackContent&lt;Value> 

static func buildPartialBlock&lt;K>(first: K) -> K

struct Conditional

A conditional result from the result builder.

