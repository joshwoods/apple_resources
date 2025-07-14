

- Security
-  SecCodeCopyStaticCode(\_:\_:\_:) 

Function

# SecCodeCopyStaticCode(\_:\_:\_:)

Returns a static code object representing the on-disk version of the given running code.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeCopyStaticCode(
    _ code: SecCode,
    _ flags: SecCSFlags,
    _ staticCode: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`code`  

A valid code object representing code running on the system.

`flags`  

Optional flags; see SecCSFlags and Code Signing Architecture Flags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`staticCode`  

On return, a static code object representing the code in the file system that is the origin of the code specified by the `code` parameter.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

Use the SecCodeCopyPath(_:_:_:) function to get the URL specifying the location on disk of the code represented by a code or static code object.

Many functions in the Code Signing Services API take either a static code object or a code object as an input parameter. For these functions, if you pass in a code reference, the function first translates it to a static code reference in the same manner as the SecCodeCopyStaticCode(_:_:_:) function. In each such case, the parameter description documents this behavior.

### Special Considerations

The link established by this function is generally reliable but is not guaranteed to be secure.

## See Also

### Related Documentation

func SecCodeCopyGuestWithAttributes(SecCode?, CFDictionary?, SecCSFlags, UnsafeMutablePointer&lt;SecCode?>) -> OSStatus

Asks a code host to identify one of its guests given the type and value of specific attributes of the guest code.

func SecCodeCopyHost(SecCode, SecCSFlags, UnsafeMutablePointer&lt;SecCode?>) -> OSStatus

Retrieves the code object for the host of specified guest code.

func SecCodeCopySelf(SecCSFlags, UnsafeMutablePointer&lt;SecCode?>) -> OSStatus

Retrieves the code object for the code making the call.

