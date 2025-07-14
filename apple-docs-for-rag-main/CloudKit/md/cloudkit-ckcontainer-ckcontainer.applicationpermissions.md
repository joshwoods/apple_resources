

- CloudKit
- CKContainer
-  CKContainer.ApplicationPermissions 

Structure

# CKContainer.ApplicationPermissions

Constants that represent the permissions that a user grants.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
struct ApplicationPermissions
```

## Topics

### Creating Permissions

init(rawValue: UInt)

Creates a premission with the specified raw value.

### Accessing Permissions

static var userDiscoverability: CKContainer.ApplicationPermissions

The user is discoverable using their email address.

Deprecated

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

### Requesting and Determining App Permissions

func requestApplicationPermission(CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Prompts the user to authorize the specified permission.

Deprecated

func status(forApplicationPermission: CKContainer.ApplicationPermissions, completionHandler: (CKContainer.ApplicationPermissionStatus, (any Error)?) -> Void)

Determines the authorization status of the specified permission.

Deprecated

enum Application

A collection of types for app permissions.

typealias ApplicationPermissionBlock

A closure that processes the outcome of a permissions request.

Deprecated

enum ApplicationPermissionStatus

Constants that represent the status of a permission.

Deprecated

