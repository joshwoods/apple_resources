

- Security
-  SecRequirementCreateWithString(\_:\_:\_:) 

Function

# SecRequirementCreateWithString(\_:\_:\_:)

Creates a code requirement object by compiling a valid text representation of a code requirement.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecRequirementCreateWithString(
    _ text: CFString,
    _ flags: SecCSFlags,
    _ requirement: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`text`  

The text form of a code requirement.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`requirement`  

On return, contains a code requirement object that implements the conditions described in the text.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

Code requirements and the code signing requirement language are documented in Code Signing Guide.

If you use the SecRequirementCreateWithString(_:_:_:) function to create a code requirement object from a text string and later use the SecRequirementCopyString(_:_:_:) function to convert the object back to a string, the reconstituted text may differ in formatting, contain different source comments, and perform its validation functions in different order from the original. However, it is guaranteed that that the reconstituted text is functionally identical to the original. That is, recompiling the text using SecRequirementCreateWithString(_:_:_:) will produce a code requirement object that behaves identically to the first one you created.

