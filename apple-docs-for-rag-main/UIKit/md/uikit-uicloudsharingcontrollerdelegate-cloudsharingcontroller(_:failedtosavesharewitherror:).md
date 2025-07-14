

- UIKit
- UICloudSharingControllerDelegate
-  cloudSharingController(\_:failedToSaveShareWithError:) 

Instance Method

# cloudSharingController(\_:failedToSaveShareWithError:)

Tells the delegate that the CloudKit sharing controller failed to save the share record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func cloudSharingController(
    _ csc: UICloudSharingController,
    failedToSaveShareWithError error: any Error
)
```

**Required**

## Discussion

Implement this method to receive a notification from the UICloudSharingController instance after it fails to save changes to the CKShare record.

## See Also

### Processing shared items

func cloudSharingControllerDidStopSharing(UICloudSharingController)

Tells the delegate that the user has stopped sharing the record.

func cloudSharingControllerDidSaveShare(UICloudSharingController)

Tells the delegate that the CloudKit sharing controller saved the share record.

