

- Core Bluetooth
- CBAttributePermissions
-  writeEncryptionRequired 

Type Property

# writeEncryptionRequired

A permission that indicates only trusted devices can write the attribute’s value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var writeEncryptionRequired: CBAttributePermissions { get }
```

## See Also

### Permissions

static var readable: CBAttributePermissions

A permission that indicates a peripheral can read the attribute’s value.

static var writeable: CBAttributePermissions

A permission that indicates a peripheral can write the attribute’s value.

static var readEncryptionRequired: CBAttributePermissions

A permission that indicates only trusted devices can read the attribute’s value.

