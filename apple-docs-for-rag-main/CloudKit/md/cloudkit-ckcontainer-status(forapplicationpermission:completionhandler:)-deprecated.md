

- CloudKit
- CKContainer
-  status(forApplicationPermission:completionHandler:) Deprecated

Instance Method

# status(forApplicationPermission:completionHandler:)

Determines the authorization status of the specified permission.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.0–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
func status(
    forApplicationPermission applicationPermission: CKContainer.ApplicationPermissions,
    completionHandler: @escaping (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void
)
```

``` source
func applicationPermissionStatus(for applicationPermission: CKContainer.ApplicationPermissions) async throws -> CKContainer.ApplicationPermissionStatus
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Parameters 

`applicationPermission`  

The permission to check. For a list of possible values, see CKContainer.ApplicationPermissions.

`completionHandler`  

The handler to execute with the outcome.

## Discussion

Use this method to determine the extra capabilities that the user grants to your app. If your app doesn’t have a specific permission, calling this method yields CKContainer.ApplicationPermissionStatus.initialState. In response, call the requestApplicationPermission(_:completionHandler:) method to prompt the user to provide their permission.

## See Also

### Requesting and Determining App Permissions

func requestApplicationPermission(CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Prompts the user to authorize the specified permission.

Deprecated

enum Application

A collection of types for app permissions.

struct ApplicationPermissions

Constants that represent the permissions that a user grants.

typealias ApplicationPermissionBlock

A closure that processes the outcome of a permissions request.

Deprecated

enum ApplicationPermissionStatus

Constants that represent the status of a permission.

Deprecated

