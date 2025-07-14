

- SwiftUI
- NSHostingView
-  isAccessibilityElement() 

Instance Method

# isAccessibilityElement()

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func isAccessibilityElement() -> Bool
```

## See Also

### Managing accessibility behaviors

var accessibilityFocusedUIElement: Any?

func accessibilityChildren() -> [Any]?

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

func accessibilityHitTest(NSPoint) -> Any?

func accessibilityRole() -> NSAccessibility.Role?

func accessibilitySubrole() -> NSAccessibility.Subrole?

