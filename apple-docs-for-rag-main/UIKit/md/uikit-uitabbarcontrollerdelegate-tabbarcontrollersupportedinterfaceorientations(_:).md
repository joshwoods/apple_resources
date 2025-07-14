

- UIKit
- UITabBarControllerDelegate
-  tabBarControllerSupportedInterfaceOrientations(\_:) 

Instance Method

# tabBarControllerSupportedInterfaceOrientations(\_:)

Called to allow the delegate to provide the complete set of supported interface orientations for the tab bar controller.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+

``` source
@MainActor
optional func tabBarControllerSupportedInterfaceOrientations(_ tabBarController: UITabBarController) -> UIInterfaceOrientationMask
```

## Parameters 

`tabBarController`  

The tab bar controller that is asking the delegate object for the supported interface orientations.

## Return Value

One of the UIInterfaceOrientationMask constants that represents the set of interface orientations supported by the tab bar controller.

## See Also

### Related Documentation

var supportedInterfaceOrientations: UIInterfaceOrientationMask

The interface orientations that the view controller supports.

### Overriding view rotation settings

func tabBarControllerPreferredInterfaceOrientationForPresentation(UITabBarController) -> UIInterfaceOrientation

Called to allow the delegate to provide the preferred orientation for presentation of the tab bar controller.

