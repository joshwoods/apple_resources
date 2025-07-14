

- Security
-  SecCodeCopyHost(\_:\_:\_:) 

Function

# SecCodeCopyHost(\_:\_:\_:)

Retrieves the code object for the host of specified guest code.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeCopyHost(
    _ guest: SecCode,
    _ flags: SecCSFlags,
    _ host: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`guest`  

A valid code object representing code running on the system as the guest of other code.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`host`  

On return, the code object of the host of the code specified in the `guest` parameter.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

Host code acts as the supervisor and controller of its guest code and is the ultimate authority on the dynamic validity and status of its guests.

