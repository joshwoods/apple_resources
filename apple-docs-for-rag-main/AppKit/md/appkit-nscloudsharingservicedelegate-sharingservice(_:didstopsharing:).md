

- AppKit
- NSCloudSharingServiceDelegate
-  sharingService(\_:didStopSharing:) 

Instance Method

# sharingService(\_:didStopSharing:)

Tells the delegate when the user stops sharing the CloudKit share.

macOS 10.8+

``` source
optional func sharingService(
    _ sharingService: NSSharingService,
    didStopSharing share: CKShare
)
```

## Parameters 

`sharingService`  

The cloud-sharing service that invokes this delegate method.

`share`  

The share the user is no longer sharing.

## Discussion

The cloud-sharing service invokes this method after it deletes the share on the server. The `share` parameter is the most recent state of the share before the service deletes it.

## See Also

### Managing the Cloud-Sharing Service

func sharingService(NSSharingService, didCompleteForItems: [Any], error: (any Error)?)

Tells the delegate when the cloud-sharing service completes.

func sharingService(NSSharingService, didSave: CKShare)

Tells the delegate when the cloud-sharing service saves the CloudKit share.

func options(for: NSSharingService, share: NSItemProvider) -> NSSharingService.CloudKitOptions

Asks the delegate for the participant options for the cloud-sharing service.

struct CloudKitOptions

Constants that describe how a participant can configure a CloudKit share.

