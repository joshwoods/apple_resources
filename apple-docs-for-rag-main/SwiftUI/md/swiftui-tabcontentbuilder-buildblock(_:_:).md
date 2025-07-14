

- SwiftUI
- TabContentBuilder
-  buildBlock(\_:\_:) 

Type Method

# buildBlock(\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func buildBlock(
    _ c0: C0,
    _ c1: C1
) -> some TabContent where TabValue == C0.TabValue, C0 : TabContent, C1 : TabContent, C0.TabValue == C1.TabValue
```

Available when `TabValue` conforms to `Hashable`.

