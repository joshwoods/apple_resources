

- CloudKit
- CKContainer
-  CKContainer.ApplicationPermissionBlock Deprecated

Type Alias

# CKContainer.ApplicationPermissionBlock

A closure that processes the outcome of a permissions request.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.10–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
typealias ApplicationPermissionBlock = (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Discussion

When you request or determine the status of a permission, use this closure to process the result. The closure has no return value and takes the following parameters:

- The permission’s status. For a list of possible values, see CKContainer.ApplicationPermissionStatus.

- An error if the system can’t fulfill the request, or `nil` if it successfully determines the status.

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

enum ApplicationPermissionStatus

Constants that represent the status of a permission.

Deprecated

