

- Swift Charts
- AxisMarkBuilder
-  buildIf(\_:) 

Type Method

# buildIf(\_:)

Provides support for “if” statements in multi-statement closures, producing an optional axis content that is visible only when the condition evaluates to `true`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildIf(_ content: T?) -> T? where T : AxisMark
```

