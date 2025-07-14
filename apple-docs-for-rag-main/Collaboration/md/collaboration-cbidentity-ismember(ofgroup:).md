

- Collaboration
- CBIdentity
-  isMember(ofGroup:) 

Instance Method

# isMember(ofGroup:)

Returns a Boolean value indicating whether the identity is a member of the specified group.

macOS 10.5+

``` source
func isMember(ofGroup group: CBGroupIdentity) -> Bool
```

## Parameters 

`group`  

The group to check for membership.

## Return Value

true if the identity is a member of the group; false if it is not.

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

var posixName: String

Returns the POSIX name of the identity.

var uuidString: String

Returns the UUID of the identity as a string.

Deprecated

