

- Core Foundation
- CFFileSecurityClearOptions
-  mode 

Type Property

# mode

Clear the file’s mode (POSIX permissions).

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var mode: CFFileSecurityClearOptions { get }
```

## See Also

### Constants

static var accessControlList: CFFileSecurityClearOptions

Clear the access control list.

static var group: CFFileSecurityClearOptions

Clear the (POSIX) group ID.

static var groupUUID: CFFileSecurityClearOptions

Clear the group UUID (for the access control list).

static var owner: CFFileSecurityClearOptions

Clear the (POSIX) owner ID.

static var ownerUUID: CFFileSecurityClearOptions

Clear the owner UUID (for the access control list).

