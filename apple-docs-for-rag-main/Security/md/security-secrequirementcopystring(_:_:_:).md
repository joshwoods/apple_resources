

- Security
-  SecRequirementCopyString(\_:\_:\_:) 

Function

# SecRequirementCopyString(\_:\_:\_:)

Converts a code requirement object into text form.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecRequirementCopyString(
    _ requirement: SecRequirement,
    _ flags: SecCSFlags,
    _ text: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`requirement`  

A valid code requirement object.

`flags`  

Optional flags; see SecCSFlags for possible values. Pass kSecCSDefaultFlags for standard behavior.

`text`  

On return, a text representation of the code requirement.

## Return Value

A result code. See Code Signing Services Result Codes.

## Discussion

If you use the SecRequirementCreateWithString(_:_:_:) or SecRequirementCreateWithStringAndErrors(_:_:_:_:) function to create a code requirement object from a text string and later use the SecRequirementCopyString(_:_:_:) function to convert the object back to a string, the reconstituted text may differ in formatting, contain different source comments, and perform its validation functions in different order from the original. However, it is guaranteed that that the reconstituted text is functionally identical to the original. That is, recompiling the text using SecRequirementCreateWithString(_:_:_:) will produce a code requirement object that behaves identically to the first one you created.

