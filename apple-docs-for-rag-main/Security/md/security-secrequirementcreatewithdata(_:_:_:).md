

- Security
-  SecRequirementCreateWithData(\_:\_:\_:) 

Function

# SecRequirementCreateWithData(\_:\_:\_:)

Creates a code requirement object from the binary form of a code requirement.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecRequirementCreateWithData(
    _ data: CFData,
    _ flags: SecCSFlags,
    _ requirement: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`data`  

A binary blob created earlier from a valid code requirement object by calling the SecRequirementCopyData(_:_:_:) function.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`requirement`  

On return, contains a code requirement object that behaves identically to the one from which the data blob was obtained.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

You can use the SecRequirementCopyData(_:_:_:) function to convert a code requirement object to a binary blob, and store the blob in any form you wish. When you are ready to use the code requirement in another function call, you can use the SecRequirementCreateWithData(_:_:_:) function to convert it back to a code requirement object.

