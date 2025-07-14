

- UIKit
-  UICloudSharingControllerDelegate 

Protocol

# UICloudSharingControllerDelegate

The protocol you implement to provide additional information to, and receive notifications from, the CloudKit sharing controller.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UICloudSharingControllerDelegate : NSObjectProtocol
```

## Overview

Implement an object that conforms to the UICloudSharingControllerDelegate protocol when you want to:

- Configure a UICloudSharingController instance.

- Receive notifications from a UICloudSharingController instance as it attempts to save or remove the CKShare record based on user interactions on the Invitation and People screens.

## Topics

### Configuring the view controller

func itemTitle(for: UICloudSharingController) -> String?

Asks the delegate for the title to display on the invitation screen.

**Required**

func itemType(for: UICloudSharingController) -> String?

Asks the delegate for the Uniform Type Identifier (UTI) of the item.

func itemThumbnailData(for: UICloudSharingController) -> Data?

Asks the delegate for the thumbnail image data to display on the invitation.

### Processing shared items

func cloudSharingController(UICloudSharingController, failedToSaveShareWithError: any Error)

Tells the delegate that the CloudKit sharing controller failed to save the share record.

**Required**

func cloudSharingControllerDidStopSharing(UICloudSharingController)

Tells the delegate that the user has stopped sharing the record.

func cloudSharingControllerDidSaveShare(UICloudSharingController)

Tells the delegate that the CloudKit sharing controller saved the share record.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the cloud sharing controller behavior

var delegate: (any UICloudSharingControllerDelegate)?

A reference to an object that conforms to the CloudKit sharing controller delegate protocol.

