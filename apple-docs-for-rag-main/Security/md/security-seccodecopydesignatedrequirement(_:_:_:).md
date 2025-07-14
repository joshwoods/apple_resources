

- Security
-  SecCodeCopyDesignatedRequirement(\_:\_:\_:) 

Function

# SecCodeCopyDesignatedRequirement(\_:\_:\_:)

Retrieves the designated code requirement of signed code.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeCopyDesignatedRequirement(
    _ code: SecStaticCode,
    _ flags: SecCSFlags,
    _ requirement: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`code`  

The code or static code object for which you want the designated requirement. If you provide a code object, the function processes it in the same manner as the SecCodeCopyStaticCode(_:_:_:) function.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`requirement`  

On return, the code’s designated requirement. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

The designated requirement is the internal code requirement that the code specifies as the way to identify it. See Code Signing Guide for a discussion of code requirements and designated requirements.

If the code contains an explicit designated requirement, a copy of that is returned. If it doesn’t, a designated requirement is constructed from the code’s signing authority and its embedded unique identifier. No designated requirement can be obtained from unsigned code. Code that is modified after being signed, that has been signed improperly, or whose signature has become invalid, may or may not yield a designated requirement. This function does not validate the signature.

## See Also

### Related Documentation

func SecCodeCopySigningInformation(SecStaticCode, SecCSFlags, UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves various pieces of information from a code signature.

