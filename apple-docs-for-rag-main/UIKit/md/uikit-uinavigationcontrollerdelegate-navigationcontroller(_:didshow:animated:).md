

- UIKit
- UINavigationControllerDelegate
-  navigationController(\_:didShow:animated:) 

Instance Method

# navigationController(\_:didShow:animated:)

Notifies the delegate after the navigation controller displays a view controller’s view and navigation item properties.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func navigationController(
    _ navigationController: UINavigationController,
    didShow viewController: UIViewController,
    animated: Bool
)
```

## Parameters 

`navigationController`  

The navigation controller that is showing the view and properties of a view controller.

`viewController`  

The view controller whose view and navigation item properties are being shown.

`animated`  

true to animate the transition; otherwise, false.

## Mentioned in 

Enhancing your app with fluid transitions

## See Also

### Responding to a view controller being shown

func navigationController(UINavigationController, willShow: UIViewController, animated: Bool)

Notifies the delegate before the navigation controller displays a view controller’s view and navigation item properties.

