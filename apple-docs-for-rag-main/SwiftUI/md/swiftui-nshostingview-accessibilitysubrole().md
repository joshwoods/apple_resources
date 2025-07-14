

- SwiftUI
- NSHostingView
-  accessibilitySubrole() 

Instance Method

# accessibilitySubrole()

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func accessibilitySubrole() -> NSAccessibility.Subrole?
```

## See Also

### Managing accessibility behaviors

var accessibilityFocusedUIElement: Any?

func accessibilityChildren() -> [Any]?

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

func accessibilityHitTest(NSPoint) -> Any?

func accessibilityRole() -> NSAccessibility.Role?

func isAccessibilityElement() -> Bool

