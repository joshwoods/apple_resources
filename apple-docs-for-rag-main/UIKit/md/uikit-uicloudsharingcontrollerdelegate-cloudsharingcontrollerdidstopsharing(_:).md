

- UIKit
- UICloudSharingControllerDelegate
-  cloudSharingControllerDidStopSharing(\_:) 

Instance Method

# cloudSharingControllerDidStopSharing(\_:)

Tells the delegate that the user has stopped sharing the record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func cloudSharingControllerDidStopSharing(_ csc: UICloudSharingController)
```

## Discussion

Implement this method to receive a notification from the UICloudSharingController instance after the user who owns the CKShare record stops sharing it with all participants.

## See Also

### Processing shared items

func cloudSharingController(UICloudSharingController, failedToSaveShareWithError: any Error)

Tells the delegate that the CloudKit sharing controller failed to save the share record.

**Required**

func cloudSharingControllerDidSaveShare(UICloudSharingController)

Tells the delegate that the CloudKit sharing controller saved the share record.

