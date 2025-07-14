

- CloudKit
- CKContainer
-  CKContainer.ApplicationPermissionStatus Deprecated

Enumeration

# CKContainer.ApplicationPermissionStatus

Constants that represent the status of a permission.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.10–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
enum ApplicationPermissionStatus
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Topics

### Permission Statuses

case initialState

The app is yet to request the permission.

case couldNotComplete

An error that occurs while processing the permission request.

case denied

The user denies the permission.

case granted

The user grants the permission.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Requesting and Determining App Permissions

func requestApplicationPermission(CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Prompts the user to authorize the specified permission.

Deprecated

func status(forApplicationPermission: CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Determines the authorization status of the specified permission.

Deprecated

enum Application

A collection of types for app permissions.

struct ApplicationPermissions

Constants that represent the permissions that a user grants.

typealias ApplicationPermissionBlock

A closure that processes the outcome of a permissions request.

Deprecated

