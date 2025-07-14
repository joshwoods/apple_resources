

- CloudKit
- CKContainer
-  requestApplicationPermission(\_:completionHandler:) Deprecated

Instance Method

# requestApplicationPermission(\_:completionHandler:)

Prompts the user to authorize the specified permission.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.0–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
func requestApplicationPermission(
    _ applicationPermission: CKContainer.ApplicationPermissions,
    completionHandler: @escaping (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void
)
```

``` source
func requestApplicationPermission(_ applicationPermission: CKContainer.ApplicationPermissions) async throws -> CKContainer.ApplicationPermissionStatus
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Parameters 

`applicationPermission`  

The permission to request. This permission applies only to the current container. For a list of possible values, see CKContainer.ApplicationPermissions.

`completionHandler`  

The handler to execute with the outcome.

## Discussion

To implement social features in your app, it’s possible to correlate a user record with the user’s actual name, but your app must get permission from the user to do so. Making a user record discoverable to the contacts of that user involves calling the requestApplicationPermission(_:completionHandler:) method and asking for the userDiscoverability permission. When you call that method, CloudKit asks the user whether the user record can become discoverable. If the user grants the request, that user’s contacts can discover that user’s true identity when running the app. To discover the contacts of the current user, you use the `discoverAllContactUserInfos(completionHandler:)` method or one of several other methods to get the related user information.

The first time you request a permission on any of the user’s devices, the user receives a prompt to grant or deny the request. After the user grants or denies a permission, subsequent requests for the same permission (on the same or separate devices), don’t prompt the user again.

This method runs asynchronously, and the system calls your completion handler on an arbitary queue and provides the outcome.

## See Also

### Requesting and Determining App Permissions

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

enum ApplicationPermissionStatus

Constants that represent the status of a permission.

Deprecated

