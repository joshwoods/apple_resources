

- UIKit
- UITab
-  managingTabGroup 

Instance Property

# managingTabGroup

The managing tab group for the tab. This returns the rootmost `UITabGroup` in the tab’s parent hierarchy with an active `managingNavigationController`. This can be different to `parent` if the tab is nested in multiple levels of tab groups. If the tab does not belong to a hierarchy with a managing navigation controller, then this will return nil. Default is nil.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var managingTabGroup: UITabGroup? { get }
```

