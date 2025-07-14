

- Security
-  SecStaticCodeCreateWithPathAndAttributes(\_:\_:\_:\_:) 

Function

# SecStaticCodeCreateWithPathAndAttributes(\_:\_:\_:\_:)

Creates a static code object representing the code at a specified file system path using an attributes dictionary.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecStaticCodeCreateWithPathAndAttributes(
    _ path: CFURL,
    _ flags: SecCSFlags,
    _ attributes: CFDictionary,
    _ staticCode: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`path`  

A URL identifying the location on disk of the code for which you want a static code object. For bundles, pass a URL to the root directory of the bundle. For single files, pass a URL to the file. If you pass a URL to the main executable of a bundle, the bundle as a whole is generally recognized. Only absolute paths should be used.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`attributes`  

A CFDictionary containing additional attributes of the requested code. Possible values are defined in Code Attributes.

`staticCode`  

On return, the static code object representing the code you specified in the `path` parameter.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

A static code object is not inherently linked to running code in the system.

It is possible to create a static code object from unsigned code. Although most uses of such an object cause the function to fail and return the result code errSecCSUnsigned error, you can call the SecCodeCopyPath(_:_:_:) and SecCodeCopySigningInformation(_:_:_:) functions for such objects.

## See Also

### Related Documentation

func SecCodeCopyPath(SecStaticCode, SecCSFlags, UnsafeMutablePointer&lt;CFURL?>) -> OSStatus

Retrieves the location on disk of signed code, given a code or static code object.

func SecCodeCopyStaticCode(SecCode, SecCSFlags, UnsafeMutablePointer&lt;SecStaticCode?>) -> OSStatus

Returns a static code object representing the on-disk version of the given running code.

