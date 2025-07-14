

- Security
-  SecCodeCopySelf(\_:\_:) 

Function

# SecCodeCopySelf(\_:\_:)

Retrieves the code object for the code making the call.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeCopySelf(
    _ flags: SecCSFlags,
    _ self: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`self`  

On return, a code object representing the caller.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

A code object (that is, an object of type SecCode) represents code that is running on the system. The code can be a UNIX process, a script, an applet, a widget, or any other separately-identifiable code. You can use the code object returned by this function as input to other functions in the Code Signing Services API. This function returns a code object for the code that calls it regardless of whether the code is signed. Call the SecCodeCheckValidity(_:_:_:) or SecCodeCheckValidityWithErrors(_:_:_:_:) function to determine whether the code has a valid signature.

If the code calling this function is either a dedicated host or has called the SecHostSelectGuest function, then the host is considered to be acting as a proxy for its dedicated or selected guest and the SecCodeCopySelf(_:_:) function returns a code object for that guest. See kSecCSDedicatedHost for a discussion of dedicated hosts.

## See Also

### Related Documentation

func SecCodeCopyGuestWithAttributes(SecCode?, CFDictionary?, SecCSFlags, UnsafeMutablePointer&lt;SecCode?>) -> OSStatus

Asks a code host to identify one of its guests given the type and value of specific attributes of the guest code.

func SecCodeCopyHost(SecCode, SecCSFlags, UnsafeMutablePointer&lt;SecCode?>) -> OSStatus

Retrieves the code object for the host of specified guest code.

func SecCodeCopyStaticCode(SecCode, SecCSFlags, UnsafeMutablePointer&lt;SecStaticCode?>) -> OSStatus

Returns a static code object representing the on-disk version of the given running code.

