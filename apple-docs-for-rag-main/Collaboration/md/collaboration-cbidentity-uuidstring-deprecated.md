

- Collaboration
- CBIdentity
-  uuidString Deprecated

Instance Property

# uuidString

Returns the UUID of the identity as a string.

macOS 10.5–10.11Deprecated

``` source
var uuidString: String { get }
```

Deprecated

Use the uniqueIdentifier property instead.

## Return Value

The UUID string of the identity.

## Discussion

The UUID string is generated so it is unique across all identity authorities. When storing ACLs, one method is to store the UUID of each identity. However, it is recommended that you use a persistent data object instead (see persistentReference).

## See Also

### Getting Identity Attributes

var aliases: [String]

Returns an array of aliases (alternate names) for the identity.

var authority: CBIdentityAuthority

Returns the identity authority where the identity is stored.

var emailAddress: String?

Returns the email address of an identity.

var fullName: String

Returns the full name of the identity.

var image: NSImage?

Returns the image associated with an identity.

var isHidden: Bool

Returns a Boolean value indicating the state of the identity’s hidden property.

func isMember(ofGroup: CBGroupIdentity) -> Bool

Returns a Boolean value indicating whether the identity is a member of the specified group.

var posixName: String

Returns the POSIX name of the identity.

