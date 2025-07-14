

- SwiftUI
- NSHostingView
-  accessibilityChildrenInNavigationOrder() 

Instance Method

# accessibilityChildrenInNavigationOrder()

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?
```

## See Also

### Managing accessibility behaviors

var accessibilityFocusedUIElement: Any?

func accessibilityChildren() -> [Any]?

func accessibilityHitTest(NSPoint) -> Any?

func accessibilityRole() -> NSAccessibility.Role?

func accessibilitySubrole() -> NSAccessibility.Subrole?

func isAccessibilityElement() -> Bool

