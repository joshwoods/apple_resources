

- UIKit
- UITabBarController
- UITabBarController.Sidebar
-  navigationOverflowItems 

Instance Property

# navigationOverflowItems

Additional items to add to the overflow menu in the sidebar’s navigation bar. Setting this property to a non-nil value will force the overflow button to appear, regardless of if you provide any content in the element’s callback. Items returned are displayed directly in the presented menu. When set, the “Edit Sidebar” action will also be moved into the overflow menu after the app-provided items.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.2+

``` source
@MainActor
var navigationOverflowItems: UIDeferredMenuElement? { get set }
```

