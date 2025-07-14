

- UIKit
- UINavigationController
-  navigationBar 

Instance Property

# navigationBar

The navigation bar managed by the navigation controller.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var navigationBar: UINavigationBar { get }
```

## Discussion

It is permissible to customize the appearance of the navigation bar using the methods and properties of the UINavigationBar class but you must never change its frame, bounds, or alpha values or modify its view hierarchy directly. To show or hide the navigation bar, you should always do so through the navigation controller by changing its isNavigationBarHidden property or calling the setNavigationBarHidden(_:animated:) method.

## See Also

### Configuring navigation bars

func setNavigationBarHidden(Bool, animated: Bool)

Sets whether the navigation bar is hidden.

Customizing your app’s navigation bar

Create custom titles, prompts, and buttons in your app’s navigation bar.

