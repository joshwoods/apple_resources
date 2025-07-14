

- Security
-  SecCodeMapMemory(\_:\_:) 

Function

# SecCodeMapMemory(\_:\_:)

Asks the kernel to accept the signing information currently attached to a code object and uses it to validate memory page-ins.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeMapMemory(
    _ code: SecStaticCode,
    _ flags: SecCSFlags
) -> OSStatus
```

## Parameters 

`code`  

A code or static code object representing the signed code whose main executable should be subject to page-in validation. If you provide a code object, the function processes it in the same manner as the SecCodeCopyStaticCode(_:_:_:) function—that is, whether you provide a code object or a static code object, the function actually takes the signature from the code on disk.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

This function is for the use of code hosts that use memory mapping to manage their own code. The kernel takes the signing information attached to the code on disk specified by the `code` parameter and attaches it to the memory object. After that, it uses the signature to validate memory page-ins, updating the dynamic validity status accordingly. You can use the SecCodeCopySigningInformation(_:_:_:) function to check the code’s dynamic validity status. The attachment of the signature to the memory object affects all processes that have the main executable of this code mapped.

