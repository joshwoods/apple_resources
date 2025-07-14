

- MapKit
- MKLookAroundViewControllerDelegate
-  lookAroundViewControllerWillPresentFullScreen(\_:) 

Instance Method

# lookAroundViewControllerWillPresentFullScreen(\_:)

Tells the delegate when the view controller is about to enter full-screen mode.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
optional func lookAroundViewControllerWillPresentFullScreen(_ viewController: MKLookAroundViewController)
```

## Parameters 

`viewController`  

The MKLookAroundViewController.

## See Also

### Entering and exiting full-screen modes

func lookAroundViewControllerDidPresentFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller enters full-screen mode.

func lookAroundViewControllerWillDismissFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller is about to exit full-screen mode.

func lookAroundViewControllerDidDismissFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller exits full-screen mode.

