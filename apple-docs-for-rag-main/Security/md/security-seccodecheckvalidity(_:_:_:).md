

- Security
-  SecCodeCheckValidity(\_:\_:\_:) 

Function

# SecCodeCheckValidity(\_:\_:\_:)

Performs dynamic validation of signed code.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecCodeCheckValidity(
    _ code: SecCode,
    _ flags: SecCSFlags,
    _ requirement: SecRequirement?
) -> OSStatus
```

## Parameters 

`code`  

The code object to be validated.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`requirement`  

A code requirement specifying additional conditions the code must satisfy to be considered valid. Specify `NULL` if you don’t want to impose any additional requirements. Use the SecRequirementCreateWithString(_:_:_:) or SecRequirementCreateWithStringAndErrors(_:_:_:_:) function to create a code requirement object. See Code Signing Guide for a discussion of code requirements.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

This function obtains and verifies the signature on the code specified by the code object. It checks the validity of only those sealed components required to establish identity. For guest code, first the function checks the code object’s dynamic validity status as reported by its host, then it ensures that the code object’s host is in turn valid. For all code, it validates the code against a code requirement if one is specified. The call succeeds if all these conditions are satisfactory.

This function is secure against attempts to modify the file system source of the code object.

