

- SwiftUI
- KeyframesBuilder
-  buildEither(first:) 

Type Method

# buildEither(first:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func buildEither(first component: First) -> KeyframeTrackContentBuilder.Conditional where Value == First.Value, First : KeyframeTrackContent, Second : KeyframeTrackContent, First.Value == Second.Value
```

## See Also

### Building keyframes

static func buildArray([some KeyframeTrackContent&lt;Value>]) -> some KeyframeTrackContent&lt;Value> 

static buildBlock()

static func buildEither&lt;First, Second>(second: Second) -> KeyframeTrackContentBuilder&lt;Value>.Conditional&lt;Value, First, Second>

static buildExpression(_:)

Keyframes

static buildFinalResult(_:)

static buildPartialBlock(accumulated:next:)

static buildPartialBlock(first:)

