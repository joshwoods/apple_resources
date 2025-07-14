

- UIKit
- UIViewController
-  setNeedsUpdateOfSupportedInterfaceOrientations() 

Instance Method

# setNeedsUpdateOfSupportedInterfaceOrientations()

Notifies the view controller about a change in supported interface orientations or preferred interface orientation for presentation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
func setNeedsUpdateOfSupportedInterfaceOrientations()
```

## Discussion

By default, this method animates any changes to orientation. To perform a nonanimated update, call this method from performWithoutAnimation(_:).

## See Also

### Configuring the view rotation settings

var supportedInterfaceOrientations: UIInterfaceOrientationMask

The interface orientations that the view controller supports.

var preferredInterfaceOrientationForPresentation: UIInterfaceOrientation

The interface orientation to use when presenting the view controller.

