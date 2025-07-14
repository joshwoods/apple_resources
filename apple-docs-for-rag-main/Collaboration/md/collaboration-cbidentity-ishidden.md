

- Collaboration
- CBIdentity
-  isHidden 

Instance Property

# isHidden

Returns a Boolean value indicating the state of the identity’s hidden property.

macOS 10.5+

``` source
var isHidden: Bool { get }
```

## Return Value

true if the identity is hidden; false if it is not.

## Discussion

A hidden identity does not show up in the Identity Picker. A hidden identity refers to system identities such as `root`, `www`, and `wheel`.

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

func isMember(ofGroup: CBGroupIdentity) -> Bool

Returns a Boolean value indicating whether the identity is a member of the specified group.

var posixName: String

Returns the POSIX name of the identity.

var uuidString: String

Returns the UUID of the identity as a string.

Deprecated

