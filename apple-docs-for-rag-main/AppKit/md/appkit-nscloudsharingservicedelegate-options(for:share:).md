

- AppKit
- NSCloudSharingServiceDelegate
-  options(for:share:) 

Instance Method

# options(for:share:)

Asks the delegate for the participant options for the cloud-sharing service.

macOS 10.12+

``` source
optional func options(
    for cloudKitSharingService: NSSharingService,
    share provider: NSItemProvider
) -> NSSharingService.CloudKitOptions
```

## Parameters 

`cloudKitSharingService`  

The cloud-sharing service that invokes this delegate method.

`provider`  

The item provider that supplies the share to the service.

## Discussion

Use this method to specify whether the share is public or private. The options you return also determine any permissions that the share’s participants have. If you don’t implement this method, the cloud-sharing service uses the standard options.

## See Also

### Managing the Cloud-Sharing Service

func sharingService(NSSharingService, didCompleteForItems: [Any], error: (any Error)?)

Tells the delegate when the cloud-sharing service completes.

func sharingService(NSSharingService, didSave: CKShare)

Tells the delegate when the cloud-sharing service saves the CloudKit share.

func sharingService(NSSharingService, didStopSharing: CKShare)

Tells the delegate when the user stops sharing the CloudKit share.

struct CloudKitOptions

Constants that describe how a participant can configure a CloudKit share.

