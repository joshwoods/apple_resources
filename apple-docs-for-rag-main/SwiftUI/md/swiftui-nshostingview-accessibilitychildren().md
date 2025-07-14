

- SwiftUI
- NSHostingView
-  accessibilityChildren() 

Instance Method

# accessibilityChildren()

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func accessibilityChildren() -> [Any]?
```

## See Also

### Managing accessibility behaviors

var accessibilityFocusedUIElement: Any?

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

func accessibilityHitTest(NSPoint) -> Any?

func accessibilityRole() -> NSAccessibility.Role?

func accessibilitySubrole() -> NSAccessibility.Subrole?

func isAccessibilityElement() -> Bool

