

- SwiftUI
- NavigationSplitViewStyle
-  prominentDetail 

Type Property

# prominentDetail

A navigation split style that attempts to maintain the size of the detail content when hiding or showing the leading columns.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static var prominentDetail: ProminentDetailNavigationSplitViewStyle { get }
```

Available when `Self` is `ProminentDetailNavigationSplitViewStyle`.

## See Also

### Creating built-in styles

static var automatic: AutomaticNavigationSplitViewStyle

A navigation split style that resolves its appearance automatically based on the current context.

static var balanced: BalancedNavigationSplitViewStyle

A navigation split style that reduces the size of the detail content to make room when showing the leading column or columns.

