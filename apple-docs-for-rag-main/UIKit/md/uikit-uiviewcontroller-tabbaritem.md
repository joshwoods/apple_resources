

- UIKit
- UIViewController
-  tabBarItem 

Instance Property

# tabBarItem

The tab bar item that represents the view controller when added to a tab bar controller.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var tabBarItem: UITabBarItem! { get set }
```

## Discussion

This is a unique instance of UITabBarItem created to represent the view controller when it is a child of a tab bar controller. The first time the property is accessed, the UITabBarItem is created. Therefore, you should not access this property if you are not using a tab bar controller to display the view controller. To ensure the tab bar item is configured, you can either override this property and add code to create the bar button items when first accessed or create the items in your view controller’s initialization code.

The default value is a tab bar item that displays the view controller’s title.

## See Also

### Configuring tab bar content

var tabBarObservedScrollView: UIScrollView?

The full-screen scroll view to synchronize with a scrolling tab bar.

Deprecated

