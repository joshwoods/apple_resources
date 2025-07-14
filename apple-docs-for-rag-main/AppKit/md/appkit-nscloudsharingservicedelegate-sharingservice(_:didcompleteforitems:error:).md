

- AppKit
- NSCloudSharingServiceDelegate
-  sharingService(\_:didCompleteForItems:error:) 

Instance Method

# sharingService(\_:didCompleteForItems:error:)

Tells the delegate when the cloud-sharing service completes.

macOS 10.8+

``` source
optional func sharingService(
    _ sharingService: NSSharingService,
    didCompleteForItems items: [Any],
    error: (any Error)?
)
```

## Parameters 

`sharingService`  

The cloud-sharing service that invokes this delegate method.

`items`  

The items the service is sharing.

`error`  

If the service can’t share the items, an error that provides information about the failure; otherwise, Nil.

## Discussion

The cloud-sharing service invokes this method when the user finishes sharing or dismisses the service’s view controller. If you implement this method, the service calls it instead of the sharingService(_:didFailToShareItems:error:) and sharingService(_:didShareItems:) methods.

## See Also

### Managing the Cloud-Sharing Service

func sharingService(NSSharingService, didSave: CKShare)

Tells the delegate when the cloud-sharing service saves the CloudKit share.

func sharingService(NSSharingService, didStopSharing: CKShare)

Tells the delegate when the user stops sharing the CloudKit share.

func options(for: NSSharingService, share: NSItemProvider) -> NSSharingService.CloudKitOptions

Asks the delegate for the participant options for the cloud-sharing service.

struct CloudKitOptions

Constants that describe how a participant can configure a CloudKit share.

