

- SwiftUI
- TabViewStyle
-  grouped 

Type Property

# grouped

A tab view style that displays a tab bar that groups its tabs together.

macOS 15.0+

``` source
@MainActor @preconcurrency
static var grouped: GroupedTabViewStyle { get }
```

Available when `Self` is `GroupedTabViewStyle`.

## Discussion

To apply this style to a tab view, or to a view that contains tab views, use the tabViewStyle(_:) modifier.

