

- Security
-  SecACLCopyAuthorizations(\_:) Deprecated

Function

# SecACLCopyAuthorizations(\_:)

Retrieves the authorization tags of a given ACL entry.

macOS 10.7–10.10Deprecated

``` source
func SecACLCopyAuthorizations(_ acl: SecACL) -> CFArray
```

Deprecated

SecKeychain is deprecated

## Parameters 

`acl`  

The ACL entry from which you wish to retrieve the authorization tags.

## Return Value

An array containing the authorizations for this entry. In Objective-C, free this object with a call to the CFRelease method when you are done with it.

## Discussion

An ACL instance includes a list of trusted apps, the name of the keychain item as it appears in user prompts, the prompt selector flag, and a list of one or more operations to which this ACL entry applies. Use this method to retrieve the list of operations for an ACL entry. Use the SecACLCopyContents(_:_:_:_:) method to retrieve the other information.

The SecACLCopyAuthorizations(_:) method returns an error if there are more tags to return than the number of elements you allocated in the `tags` array. A 20-element array should suffice for most purposes; however, you can test for the errSecBufferTooSmall error and increase the size of the array before calling the method again if necessary. Alternatively, you can call the method with a tag count of `0`, read the value returned in the `tagCount` parameter, and then call the method again using that value.

