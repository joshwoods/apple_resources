

- UIKit
- UIViewController
-  preferredInterfaceOrientationForPresentation 

Instance Property

# preferredInterfaceOrientationForPresentation

The interface orientation to use when presenting the view controller.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var preferredInterfaceOrientationForPresentation: UIInterfaceOrientation { get }
```

## Return Value

The interface orientation with which to present the view controller.

## Discussion

The system calls this method when presenting the view controller full screen. When your view controller supports two or more orientations but the content appears best in one of those orientations, override this method and return the preferred orientation.

If your view controller implements this method, your view controller’s view is shown in the preferred orientation (although it can later be rotated to another supported rotation). If you do not implement this method, the system presents the view controller using the current orientation of the status bar.

## See Also

### Configuring the view rotation settings

var supportedInterfaceOrientations: UIInterfaceOrientationMask

The interface orientations that the view controller supports.

func setNeedsUpdateOfSupportedInterfaceOrientations()

Notifies the view controller about a change in supported interface orientations or preferred interface orientation for presentation.

