

- SwiftUI
- NSHostingView
-  accessibilityFocusedUIElement 

Instance Property

# accessibilityFocusedUIElement

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic var accessibilityFocusedUIElement: Any? { get }
```

## See Also

### Managing accessibility behaviors

func accessibilityChildren() -> [Any]?

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

func accessibilityHitTest(NSPoint) -> Any?

func accessibilityRole() -> NSAccessibility.Role?

func accessibilitySubrole() -> NSAccessibility.Subrole?

func isAccessibilityElement() -> Bool

