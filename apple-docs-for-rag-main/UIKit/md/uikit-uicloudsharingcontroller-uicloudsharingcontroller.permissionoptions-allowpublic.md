

- UIKit
- UICloudSharingController
- UICloudSharingController.PermissionOptions
-  allowPublic 

Type Property

# allowPublic

The option that grants access to anyone who has the share link.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var allowPublic: UICloudSharingController.PermissionOptions { get }
```

## Discussion

To give the user the option to allow anyone to access the shared data, include the allowPublic option when setting the availablePermissions property on the UICloudSharingController instance.

## See Also

### Constants

static var allowPrivate: UICloudSharingController.PermissionOptions

The option that restricts access to people who have been invited.

static var allowReadOnly: UICloudSharingController.PermissionOptions

The option that gives participants read-only permission to the shared data.

static var allowReadWrite: UICloudSharingController.PermissionOptions

The option that gives participants read/write permission to the shared data.

