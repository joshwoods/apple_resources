

- UIKit
- UITabBar
-  delegate 

Instance Property

# delegate

The tab bar’s delegate object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UITabBarDelegate)? { get set }
```

## Discussion

Use the delegate to track the selection of tab bar items and to respond to the user customization of the tab bar. The default value of this property is `nil`.

For more information on how to implement the methods of this protocol, see UITabBarDelegate.

## See Also

### Customizing the tab bar behavior

protocol UITabBarDelegate

The UITabBarDelegate protocol defines optional methods for a delegate of a UITabBar object. The UITabBar class provides the ability for the user to reorder, remove, and add items to the tab bar; this process is referred to as customizing the tab bar. The tab bar delegate receives messages when customizing occurs.

