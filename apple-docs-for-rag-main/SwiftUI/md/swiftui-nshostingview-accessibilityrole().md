

- SwiftUI
- NSHostingView
-  accessibilityRole() 

Instance Method

# accessibilityRole()

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func accessibilityRole() -> NSAccessibility.Role?
```

## See Also

### Managing accessibility behaviors

var accessibilityFocusedUIElement: Any?

func accessibilityChildren() -> [Any]?

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

func accessibilityHitTest(NSPoint) -> Any?

func accessibilitySubrole() -> NSAccessibility.Subrole?

func isAccessibilityElement() -> Bool

