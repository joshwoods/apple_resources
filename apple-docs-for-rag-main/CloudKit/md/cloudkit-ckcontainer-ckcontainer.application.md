

- CloudKit
- CKContainer
-  CKContainer.Application 

Enumeration

# CKContainer.Application

A collection of types for app permissions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
enum Application
```

## Topics

### Container Application Types

typealias Permissions

A type that represents the permissions that a user grants.

typealias PermissionBlock

A type that represents a handler that processes the outcome of a permission’s request.

typealias PermissionStatus

A type that represents the status of a permission.

## See Also

### Requesting and Determining App Permissions

func requestApplicationPermission(CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Prompts the user to authorize the specified permission.

Deprecated

func status(forApplicationPermission: CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Determines the authorization status of the specified permission.

Deprecated

struct ApplicationPermissions

Constants that represent the permissions that a user grants.

typealias ApplicationPermissionBlock

A closure that processes the outcome of a permissions request.

Deprecated

enum ApplicationPermissionStatus

Constants that represent the status of a permission.

Deprecated

