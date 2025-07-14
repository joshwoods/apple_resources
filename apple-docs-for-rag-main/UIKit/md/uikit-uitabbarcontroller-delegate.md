

- UIKit
- UITabBarController
-  delegate 

Instance Property

# delegate

The tab bar controller’s delegate object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UITabBarControllerDelegate)? { get set }
```

## Discussion

You can use the delegate object to track changes to the items in the tab bar and to monitor the selection of tabs. The delegate object you provide should conform to the UITabBarControllerDelegate protocol. The default value for this property is `nil`.

## See Also

### Customizing the tab bar behavior

protocol UITabBarControllerDelegate

A set of methods you implement to customize the behavior of a tab bar.

