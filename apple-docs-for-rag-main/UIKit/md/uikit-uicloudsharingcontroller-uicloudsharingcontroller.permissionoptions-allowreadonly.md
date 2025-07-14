

- UIKit
- UICloudSharingController
- UICloudSharingController.PermissionOptions
-  allowReadOnly 

Type Property

# allowReadOnly

The option that gives participants read-only permission to the shared data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var allowReadOnly: UICloudSharingController.PermissionOptions { get }
```

## Discussion

To give the user the option to prevent other people from editing the shared data, include the allowReadOnly option when setting the availablePermissions property on the UICloudSharingController instance.

## See Also

### Constants

static var allowPublic: UICloudSharingController.PermissionOptions

The option that grants access to anyone who has the share link.

static var allowPrivate: UICloudSharingController.PermissionOptions

The option that restricts access to people who have been invited.

static var allowReadWrite: UICloudSharingController.PermissionOptions

The option that gives participants read/write permission to the shared data.

