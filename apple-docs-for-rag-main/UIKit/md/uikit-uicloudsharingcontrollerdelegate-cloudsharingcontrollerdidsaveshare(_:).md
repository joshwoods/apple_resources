

- UIKit
- UICloudSharingControllerDelegate
-  cloudSharingControllerDidSaveShare(\_:) 

Instance Method

# cloudSharingControllerDidSaveShare(\_:)

Tells the delegate that the CloudKit sharing controller saved the share record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func cloudSharingControllerDidSaveShare(_ csc: UICloudSharingController)
```

## Discussion

Implement this method to receive a notification from the UICloudSharingController instance after it saves changes to the CKShare record.

## See Also

### Processing shared items

func cloudSharingController(UICloudSharingController, failedToSaveShareWithError: any Error)

Tells the delegate that the CloudKit sharing controller failed to save the share record.

**Required**

func cloudSharingControllerDidStopSharing(UICloudSharingController)

Tells the delegate that the user has stopped sharing the record.

