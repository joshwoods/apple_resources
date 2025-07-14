

- SwiftUI
- KeyframesBuilder
-  buildPartialBlock(first:) 

Type Method

# buildPartialBlock(first:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func buildPartialBlock(first: Content) -> Content where Value == Content.Value, Content : Keyframes
```

Show all declarations

## See Also

### Building keyframes

static func buildArray([some KeyframeTrackContent&lt;Value>]) -> some KeyframeTrackContent&lt;Value> 

static buildBlock()

static func buildEither&lt;First, Second>(first: First) -> KeyframeTrackContentBuilder&lt;Value>.Conditional&lt;Value, First, Second>

static func buildEither&lt;First, Second>(second: Second) -> KeyframeTrackContentBuilder&lt;Value>.Conditional&lt;Value, First, Second>

static buildExpression(_:)

Keyframes

static buildFinalResult(_:)

static buildPartialBlock(accumulated:next:)

