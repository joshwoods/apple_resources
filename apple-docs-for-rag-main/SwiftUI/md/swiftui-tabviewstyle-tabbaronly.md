

- SwiftUI
- TabViewStyle
-  tabBarOnly 

Type Property

# tabBarOnly

A tab view style that displays a tab bar when possible.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
static var tabBarOnly: TabBarOnlyTabViewStyle { get }
```

Available when `Self` is `TabBarOnlyTabViewStyle`.

## Discussion

To apply this style to a tab view, or to a view that contains tab views, use the tabViewStyle(_:) modifier.

