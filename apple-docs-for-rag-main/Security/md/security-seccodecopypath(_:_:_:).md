

- Security
-  SecCodeCopyPath(\_:\_:\_:) 

Function

# SecCodeCopyPath(\_:\_:\_:)

Retrieves the location on disk of signed code, given a code or static code object.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeCopyPath(
    _ staticCode: SecStaticCode,
    _ flags: SecCSFlags,
    _ path: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`staticCode`  

The code or static code object whose code you wish to locate. If you provide a code object, the function processes it in the same manner as the SecCodeCopyStaticCode(_:_:_:) function.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`path`  

On return, provides a URL identifying the location on disk of the code or static code object. For single files, the URL points to the file. For bundles, it points to the directory containing the entire bundle. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Code Signing Services Result Codes.

## See Also

### Related Documentation

func SecCodeCopySigningInformation(SecStaticCode, SecCSFlags, UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves various pieces of information from a code signature.

