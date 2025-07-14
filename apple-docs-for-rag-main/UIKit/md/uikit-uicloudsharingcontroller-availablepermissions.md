

- UIKit
- UICloudSharingController
-  availablePermissions 

Instance Property

# availablePermissions

A combination of permission and access options made available to the user when viewing screens presented by the CloudKit sharing controller.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var availablePermissions: UICloudSharingController.PermissionOptions { get set }
```

## Discussion

The UICloudSharingController user interface displays permission options to the user. The user selects the options based on how the data should be shared. For instance, the user can decide to share the data publicly or privately by selecting the corresponding option.

Setting the availablePermissions property on UICloudSharingController to one or more UICloudSharingController.PermissionOptions options tells the controller which options to present to the user. If you want, for example, to let the user decide whether to share the data publicly or privately, you specify the allowPublic and allowPrivate options for availablePermissions. This tells the controller to display both options to the user.

Specifying no options for availablePermissions tells UICloudSharingController to display all options to the user.

- Swift
- Objective-C

```
// Allow only the invited participants and read/write permission options.
cloudSharingController.availablePermissions = [.allowPrivate, .allowReadWrite]
```

```
// Allow only the invited participants and read/write permission options.
[cloudSharingController setAvailablePermissions:UICloudSharingPermissionAllowPrivate | UICloudSharingPermissionAllowReadWrite];
```

### Display groupings

The UICloudSharingController displays the permission options to the user based on the options set in the availablePermissions property. The user interface displays the options in two groups, access options group and permission options group. The allowPublic and allowPrivate options control the display of the access options group, while the allowReadOnly and allowReadWrite options control the display of the permission options group.

### Complementary options

The allowPrivate and allowPublic options are complementary. If you exclude one, the access options group is omitted from the UICloudSharingController user interface, and the share access setting defaults to the included option. This prevents the user from changing the access rights to the share. For instance, to always force a private share, you include the allowPrivate access option while excluding allowPublic when setting the availablePermissions property. The controller sets the share’s access rights to private and removes the access options group from the user interface, preventing the user from changing the setting.

Similarly, allowReadOnly and allowReadWrite complement each other. Excluding one removes the permission options group from the user interface, and the share permission setting defaults to the included UICloudSharingController.PermissionOptions option.

## See Also

### Configuring the permissions

struct PermissionOptions

A set of options that determine the permission options available to the user when viewing the Cloud sharing controller screens.

