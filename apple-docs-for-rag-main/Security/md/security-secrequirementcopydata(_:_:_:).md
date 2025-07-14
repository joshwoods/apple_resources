

- Security
-  SecRequirementCopyData(\_:\_:\_:) 

Function

# SecRequirementCopyData(\_:\_:\_:)

Extracts a binary form of a code requirement from a code requirement object.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecRequirementCopyData(
    _ requirement: SecRequirement,
    _ flags: SecCSFlags,
    _ data: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`requirement`  

A valid code requirement object.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`data`  

On return, the code requirement in the form of a binary blob.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

You can extract the binary blob from the CFData object and store it in any form you wish. Use of this function is the only publicly supported way to get such a data blob. You can use the SecRequirementCreateWithData(_:_:_:) function to convert it back to a code requirement object.

