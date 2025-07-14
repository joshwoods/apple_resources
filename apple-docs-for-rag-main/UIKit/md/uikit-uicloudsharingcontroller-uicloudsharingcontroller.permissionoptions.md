

- UIKit
- UICloudSharingController
-  UICloudSharingController.PermissionOptions 

Structure

# UICloudSharingController.PermissionOptions

A set of options that determine the permission options available to the user when viewing the Cloud sharing controller screens.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct PermissionOptions
```

## Overview

These options are used when setting the availablePermissions property on the UICloudSharingController instance. This property determines which permission options are presented to the user in the controller’s user interface.

## Topics

### Constants

static var allowPublic: UICloudSharingController.PermissionOptions

The option that grants access to anyone who has the share link.

static var allowPrivate: UICloudSharingController.PermissionOptions

The option that restricts access to people who have been invited.

static var allowReadOnly: UICloudSharingController.PermissionOptions

The option that gives participants read-only permission to the shared data.

static var allowReadWrite: UICloudSharingController.PermissionOptions

The option that gives participants read/write permission to the shared data.

### Initializers

init(rawValue: UInt)

Creates a new permission option set with the given raw integer value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring the permissions

var availablePermissions: UICloudSharingController.PermissionOptions

A combination of permission and access options made available to the user when viewing screens presented by the CloudKit sharing controller.

