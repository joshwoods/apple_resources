

- SwiftUI
-  AccessibilityRotorContentBuilder 

Structure

# AccessibilityRotorContentBuilder

Result builder you use to generate rotor entry content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@resultBuilder
struct AccessibilityRotorContentBuilder
```

## Topics

### Building navigation content

static func buildBlock&lt;Content>(Content) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1>(C0, C1) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2>(C0, C1, C2) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3>(C0, C1, C2, C3) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4>(C0, C1, C2, C3, C4) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5>(C0, C1, C2, C3, C4, C5) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6>(C0, C1, C2, C3, C4, C5, C6) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7>(C0, C1, C2, C3, C4, C5, C6, C7) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8>(C0, C1, C2, C3, C4, C5, C6, C7, C8) -> some AccessibilityRotorContent

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9) -> some AccessibilityRotorContent

static func buildIf&lt;Content>(Content?) -> some AccessibilityRotorContent

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

## See Also

### Creating rotors

protocol AccessibilityRotorContent

Content within an accessibility rotor.

struct AccessibilityRotorEntry

A struct representing an entry in an Accessibility Rotor.

