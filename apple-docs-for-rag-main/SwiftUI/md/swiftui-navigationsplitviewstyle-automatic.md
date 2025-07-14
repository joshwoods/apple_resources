

- SwiftUI
- NavigationSplitViewStyle
-  automatic 

Type Property

# automatic

A navigation split style that resolves its appearance automatically based on the current context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static var automatic: AutomaticNavigationSplitViewStyle { get }
```

Available when `Self` is `AutomaticNavigationSplitViewStyle`.

## See Also

### Creating built-in styles

static var balanced: BalancedNavigationSplitViewStyle

A navigation split style that reduces the size of the detail content to make room when showing the leading column or columns.

static var prominentDetail: ProminentDetailNavigationSplitViewStyle

A navigation split style that attempts to maintain the size of the detail content when hiding or showing the leading columns.

