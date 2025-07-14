

- UIKit
- UITabBarControllerDelegate
-  tabBarControllerPreferredInterfaceOrientationForPresentation(\_:) 

Instance Method

# tabBarControllerPreferredInterfaceOrientationForPresentation(\_:)

Called to allow the delegate to provide the preferred orientation for presentation of the tab bar controller.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+

``` source
@MainActor
optional func tabBarControllerPreferredInterfaceOrientationForPresentation(_ tabBarController: UITabBarController) -> UIInterfaceOrientation
```

## Parameters 

`tabBarController`  

The tab bar controller that is asking the delegate object for the preferred presentation orientation.

## Return Value

The preferred orientation for presenting the tab bar controller.

## See Also

### Related Documentation

var preferredInterfaceOrientationForPresentation: UIInterfaceOrientation

The interface orientation to use when presenting the view controller.

### Overriding view rotation settings

func tabBarControllerSupportedInterfaceOrientations(UITabBarController) -> UIInterfaceOrientationMask

Called to allow the delegate to provide the complete set of supported interface orientations for the tab bar controller.

