

- Security
- Keychain services
- Access Control Lists
-  SecAccessOwnerType Values 

API Collection

# SecAccessOwnerType Values

Flags that enable you to configure ACL ownership.

Mac Catalyst 16.0+macOS 10.7+

## Topics

### Constants

var kSecUseOnlyUID: Int

The access control list should be owned by the user matching the specified user ID parameter.

var kSecUseOnlyGID: Int

The access control list should be owned by users that are members of a group matching the specified group ID parameter.

var kSecHonorRoot: Int

The access control list should treat the root user as a typical user for ownership purposes.

var kSecMatchBits: Int

The access control list should be owned by users whose ID matches the specified user ID or who are members of a group whose ID matches the specified group ID parameter.

