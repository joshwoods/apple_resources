

- SwiftUI
- NSHostingView
-  accessibilityHitTest(\_:) 

Instance Method

# accessibilityHitTest(\_:)

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func accessibilityHitTest(_ point: NSPoint) -> Any?
```

## See Also

### Managing accessibility behaviors

var accessibilityFocusedUIElement: Any?

func accessibilityChildren() -> [Any]?

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

func accessibilityRole() -> NSAccessibility.Role?

func accessibilitySubrole() -> NSAccessibility.Subrole?

func isAccessibilityElement() -> Bool

