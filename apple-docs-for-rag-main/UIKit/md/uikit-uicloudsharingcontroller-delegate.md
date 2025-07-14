

- UIKit
- UICloudSharingController
-  delegate 

Instance Property

# delegate

A reference to an object that conforms to the CloudKit sharing controller delegate protocol.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UICloudSharingControllerDelegate)? { get set }
```

## Discussion

The UICloudSharingController instance can interact with your app by way of a delegate object (an object that conforms to the UICloudSharingControllerDelegate protocol). If you provide a delegate object to the controller, the controller can notify your app of status changes to the CKShare record that happen while the user interacts with the controller’s user interface. The controller can also ask the delegate object for app-specific settings, such as a title, for display in the controller’s user interface.

Although providing a delegate object is not required, doing so ensures that, at a minimum, a meaningful title is displayed in the controller’s user interface.

## See Also

### Customizing the cloud sharing controller behavior

protocol UICloudSharingControllerDelegate

The protocol you implement to provide additional information to, and receive notifications from, the CloudKit sharing controller.

