

- AppKit
- NSCloudSharingServiceDelegate
-  sharingService(\_:didSave:) 

Instance Method

# sharingService(\_:didSave:)

Tells the delegate when the cloud-sharing service saves the CloudKit share.

macOS 10.8+

``` source
optional func sharingService(
    _ sharingService: NSSharingService,
    didSave share: CKShare
)
```

## Parameters 

`sharingService`  

The cloud-sharing service that invokes this delegate method.

`share`  

The saved CloudKit share.

## Discussion

The cloud-sharing service invokes this method when it saves changes to the share. The `share` parameter is the most recent state of the share on the server.

## See Also

### Managing the Cloud-Sharing Service

func sharingService(NSSharingService, didCompleteForItems: [Any], error: (any Error)?)

Tells the delegate when the cloud-sharing service completes.

func sharingService(NSSharingService, didStopSharing: CKShare)

Tells the delegate when the user stops sharing the CloudKit share.

func options(for: NSSharingService, share: NSItemProvider) -> NSSharingService.CloudKitOptions

Asks the delegate for the participant options for the cloud-sharing service.

struct CloudKitOptions

Constants that describe how a participant can configure a CloudKit share.

