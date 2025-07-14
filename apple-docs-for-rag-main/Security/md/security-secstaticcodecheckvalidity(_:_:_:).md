

- Security
-  SecStaticCodeCheckValidity(\_:\_:\_:) 

Function

# SecStaticCodeCheckValidity(\_:\_:\_:)

Validates a static code object.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecStaticCodeCheckValidity(
    _ staticCode: SecStaticCode,
    _ flags: SecCSFlags,
    _ requirement: SecRequirement?
) -> OSStatus
```

## Parameters 

`staticCode`  

The static code object to be validated.

`flags`  

Optional flags; see Static Code Validation Flags for possible values. Use kSecCSCheckAllArchitectures to validate all slices of a universal binary.

`requirement`  

A code requirement specifying additional conditions the code must satisfy to be considered valid. Specify `NULL` if you don’t want to impose any additional requirements. Use the SecRequirementCreateWithString(_:_:_:) or SecRequirementCreateWithStringAndErrors(_:_:_:_:) function to create a code requirement object. See Code Signing Guide for a discussion of code requirements.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

This function obtains and verifies the signature on the code specified by the code object. It checks the validity of all sealed components, including resources (if any). It validates the code against a code requirement if one is specified. The call succeeds if all these conditions are satisfactory.

This call is only secure if the code is not subject to concurrent modification, and the outcome is only valid as long as the code remains unmodified. If the underlying file system has dynamic characteristics, such as a network file system, union mount, or FUSE, you must consider how secure the code is from modification after validation.

When checking a universal binary, include the kSecCSCheckAllArchitectures flag. Otherwise the method verifies only one slice of the binary, potentially indicating success without testing all the slices. Be aware that the slices of a universal binary don’t have to be signed by the same signer for the test to pass. One slice might be ad hoc signed, for example. But the validity check doesn’t know which slice you are going to run. For example, the user might use the arch(1) command line utility to pick a 32-bit architecture even though a 64-bit architecture is available.

If you want to be sure to test a particular slice, create the static code object with the SecStaticCodeCreateWithPathAndAttributes(_:_:_:_:) method using the kSecCodeAttributeArchitecture and kSecCodeAttributeSubarchitecture attributes (if you know the architecture) or the kSecCodeAttributeUniversalFileOffset attribute (if you know the offset into the universal binary).

