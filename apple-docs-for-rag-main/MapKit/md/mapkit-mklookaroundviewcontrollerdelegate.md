

- MapKit
-  MKLookAroundViewControllerDelegate 

Protocol

# MKLookAroundViewControllerDelegate

Methods you implement to respond to changes in the LookAround view controller.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
protocol MKLookAroundViewControllerDelegate : NSObjectProtocol
```

## Topics

### Responding to scene changes

func lookAroundViewControllerWillUpdateScene(MKLookAroundViewController)

Tells the delegate that the scene is about to update.

func lookAroundViewControllerDidUpdateScene(MKLookAroundViewController)

Tells the delegate that the scene updated.

### Entering and exiting full-screen modes

func lookAroundViewControllerWillPresentFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller is about to enter full-screen mode.

func lookAroundViewControllerDidPresentFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller enters full-screen mode.

func lookAroundViewControllerWillDismissFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller is about to exit full-screen mode.

func lookAroundViewControllerDidDismissFullScreen(MKLookAroundViewController)

Tells the delegate when the view controller exits full-screen mode.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Interacting with the controller

var delegate: (any MKLookAroundViewControllerDelegate)?

An object you provide to receive events related to the user’s interaction with the LookAround view controller.

