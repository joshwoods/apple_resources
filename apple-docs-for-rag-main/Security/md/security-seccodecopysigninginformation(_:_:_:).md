

- Security
-  SecCodeCopySigningInformation(\_:\_:\_:) 

Function

# SecCodeCopySigningInformation(\_:\_:\_:)

Retrieves various pieces of information from a code signature.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeCopySigningInformation(
    _ code: SecStaticCode,
    _ flags: SecCSFlags,
    _ information: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`code`  

The code or static code object from whose signature you wish to retrieve information. If you provide a code object, the function processes it in the same manner as the SecCodeCopyStaticCode(_:_:_:) function—that is, the static code signing information is obtained from the signature on disk. Note that dynamic information (kSecCSDynamicInformation) can be obtained only for a code object, not for a static code object.

`flags`  

Specify any or all of the flags in Code Signing Information Flags to select what information to return. A basic set of values is returned regardless; specify kSecCSDefaultFlags for just those.

`information`  

On return, a dictionary containing information about the code. The contents of the dictionary depend on the flags you pass in the `flags` parameter. Regardless of flags, the kSecCodeInfoIdentifier key is always present if the code is signed and always absent if the code is unsigned. See Signing Information Dictionary Keys for descriptions of the dictionary keys. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

The amount and detail level of the data returned is controlled by the flags passed to the call.

If the code exists but is not signed, this function call succeeds and returns a dictionary that does not contain the kSecCodeInfoIdentifier key. This is the recommended way to check quickly whether code is signed if that is the only information you need. However, note that this function does not validate the signature.

If the signing data for the code is corrupt or invalid, this function may fail or it may return partial data. To ensure that only valid data is returned (and errors are raised for invalid data), you must successfully call the SecCodeCheckValidity(_:_:_:) or SecCodeCheckValidityWithErrors(_:_:_:_:) function before calling SecCodeCopySigningInformation(_:_:_:).

### Special Considerations

Some of the objects returned in the information dictionary are (retained) “live” API objects used by the code signing infrastructure. Making changes to these objects is unsupported and may cause subsequent code signing operations on the affected code to behave in undefined ways.

## See Also

### Related Documentation

func SecCodeCopyDesignatedRequirement(SecStaticCode, SecCSFlags, UnsafeMutablePointer&lt;SecRequirement?>) -> OSStatus

Retrieves the designated code requirement of signed code.

func SecCodeCopyPath(SecStaticCode, SecCSFlags, UnsafeMutablePointer&lt;CFURL?>) -> OSStatus

Retrieves the location on disk of signed code, given a code or static code object.

