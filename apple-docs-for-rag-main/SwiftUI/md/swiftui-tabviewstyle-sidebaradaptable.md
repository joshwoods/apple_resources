

- SwiftUI
- TabViewStyle
-  sidebarAdaptable 

Type Property

# sidebarAdaptable

A tab bar style that adapts to each platform.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
static var sidebarAdaptable: SidebarAdaptableTabViewStyle { get }
```

Available when `Self` is `SidebarAdaptableTabViewStyle`.

## Discussion

Tab views using the sidebar adaptable style have an appearance that varies depending on the platform:

- iPadOS displays a top tab bar that can adapt into a sidebar.

- iOS displays a bottom tab bar.

- macOS and tvOS always show a sidebar.

- visionOS shows an ornament and also shows a sidebar for secondary tabs within a TabSection.

To apply this style to a tab view, or to a view that contains tab views, use the tabViewStyle(_:) modifier.

