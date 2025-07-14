

- MapKit
- MKLookAroundViewControllerDelegate
-  lookAroundViewControllerWillDismissFullScreen(\_:) 

Instance Method

# lookAroundViewControllerWillDismissFullScreen(\_:)

Tells the delegate when the view controller is about to exit full-screen mode.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
optional func lookAroundViewControllerWillDismissFullScreen(_ viewController: MKLookAroundViewController)
```

## Parameters 

`viewController`  

The MKLookAroundViewController.

## See Also

### Entering and exiting full-screen modes

func lookAroundViewControllerWillPresentFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller is about to enter full-screen mode.

func lookAroundViewControllerDidPresentFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller enters full-screen mode.

func lookAroundViewControllerDidDismissFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller exits full-screen mode.

