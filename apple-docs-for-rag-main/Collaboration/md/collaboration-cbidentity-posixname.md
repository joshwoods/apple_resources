

- Collaboration
- CBIdentity
-  posixName 

Instance Property

# posixName

Returns the POSIX name of the identity.

macOS 10.5+

``` source
var posixName: String { get }
```

## Return Value

The POSIX name of the identity.

## Discussion

The POSIX name is also referred to as the “short name” for an identity. It can only contain the characters A-Z, a-z, 0-9, -, \_, ., and @.

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

var uuidString: String

Returns the UUID of the identity as a string.

Deprecated

