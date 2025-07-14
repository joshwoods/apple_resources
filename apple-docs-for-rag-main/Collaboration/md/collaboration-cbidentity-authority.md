

- Collaboration
- CBIdentity
-  authority 

Instance Property

# authority

Returns the identity authority where the identity is stored.

macOS 10.5+

``` source
var authority: CBIdentityAuthority { get }
```

## Return Value

The identity authority where the identity is stored.

## See Also

### Getting Identity Attributes

var aliases: [String]

Returns an array of aliases (alternate names) for the identity.

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

var uuidString: String

Returns the UUID of the identity as a string.

Deprecated

