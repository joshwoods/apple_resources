

- UIKit
- UICloudSharingController
- UICloudSharingController.PermissionOptions
-  allowPrivate 

Type Property

# allowPrivate

The option that restricts access to people who have been invited.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var allowPrivate: UICloudSharingController.PermissionOptions { get }
```

## Discussion

To give the user the option to limit access to people who have been invited, include the allowPrivate option when setting the availablePermissions property on the UICloudSharingController instance.

Note

When inviting someone, the user must provide that person’s email address or phone number. This is how the person is identified when accepting the invitation.

## See Also

### Constants

static var allowPublic: UICloudSharingController.PermissionOptions

The option that grants access to anyone who has the share link.

static var allowReadOnly: UICloudSharingController.PermissionOptions

The option that gives participants read-only permission to the shared data.

static var allowReadWrite: UICloudSharingController.PermissionOptions

The option that gives participants read/write permission to the shared data.

