

- Shared With You
- SWCollaborationView
-  cloudSharingServiceDelegate 

Instance Property

# cloudSharingServiceDelegate

A reference to an object that conforms to the cloud-sharing service delegate protocol.

macOS 13.0+

``` source
@MainActor
weak var cloudSharingServiceDelegate: (any NSCloudSharingServiceDelegate)? { get set }
```

## See Also

### Customizing the cloud-sharing behavior

var cloudSharingControllerDelegate: (any UICloudSharingControllerDelegate)?

A reference to an object that conforms to the CloudKit sharing controller delegate protocol.

