

- Swift Charts
- AxisContentBuilder
-  buildEither(second:) 

Type Method

# buildEither(second:)

Provides support for “if-else” statements in multi-statement closures, producing conditional content for the “else” branch.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildEither(second: T2) -> BuilderConditional where T1 : AxisContent, T2 : AxisContent
```

