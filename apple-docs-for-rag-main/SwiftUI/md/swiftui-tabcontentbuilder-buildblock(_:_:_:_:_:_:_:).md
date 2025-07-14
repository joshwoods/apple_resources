

- SwiftUI
- TabContentBuilder
-  buildBlock(\_:\_:\_:\_:\_:\_:\_:) 

Type Method

# buildBlock(\_:\_:\_:\_:\_:\_:\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func buildBlock(
    _ c0: C0,
    _ c1: C1,
    _ c2: C2,
    _ c3: C3,
    _ c4: C4,
    _ c5: C5,
    _ c6: C6
) -> some TabContent where TabValue == C0.TabValue, C0 : TabContent, C1 : TabContent, C2 : TabContent, C3 : TabContent, C4 : TabContent, C5 : TabContent, C6 : TabContent, C0.TabValue == C1.TabValue, C1.TabValue == C2.TabValue, C2.TabValue == C3.TabValue, C3.TabValue == C4.TabValue, C4.TabValue == C5.TabValue, C5.TabValue == C6.TabValue
```

Available when `TabValue` conforms to `Hashable`.

