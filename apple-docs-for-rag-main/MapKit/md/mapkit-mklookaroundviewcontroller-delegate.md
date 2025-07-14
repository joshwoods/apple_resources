

- MapKit
- MKLookAroundViewController
-  delegate 

Instance Property

# delegate

An object you provide to receive events related to the user’s interaction with the LookAround view controller.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@IBOutlet @MainActor
weak var delegate: (any MKLookAroundViewControllerDelegate)? { get set }
```

## See Also

### Interacting with the controller

protocol MKLookAroundViewControllerDelegate

Methods you implement to respond to changes in the LookAround view controller.

