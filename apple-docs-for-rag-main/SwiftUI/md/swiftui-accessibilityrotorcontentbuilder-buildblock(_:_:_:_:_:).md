

- SwiftUI
- AccessibilityRotorContentBuilder
-  buildBlock(\_:\_:\_:\_:\_:) 

Type Method

# buildBlock(\_:\_:\_:\_:\_:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func buildBlock(
    _ c0: C0,
    _ c1: C1,
    _ c2: C2,
    _ c3: C3,
    _ c4: C4
) -> some AccessibilityRotorContent where C0 : AccessibilityRotorContent, C1 : AccessibilityRotorContent, C2 : AccessibilityRotorContent, C3 : AccessibilityRotorContent, C4 : AccessibilityRotorContent
```

## See Also

### Building navigation content

static func buildBlock&lt;Content>(Content) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1>(C0, C1) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2>(C0, C1, C2) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3>(C0, C1, C2, C3) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5>(C0, C1, C2, C3, C4, C5) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6>(C0, C1, C2, C3, C4, C5, C6) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7>(C0, C1, C2, C3, C4, C5, C6, C7) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8>(C0, C1, C2, C3, C4, C5, C6, C7, C8) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9) -> some AccessibilityRotorContent

static func buildIf&lt;Content>(Content?) -> some AccessibilityRotorContent

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

