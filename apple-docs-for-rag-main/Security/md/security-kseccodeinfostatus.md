

- Security
-  kSecCodeInfoStatus 

Global Variable

# kSecCodeInfoStatus

A key whose value is the set of code status flags for the running code.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoStatus: CFString
```

## Discussion

The value is a CFNumber object. This is a snapshot taken at the time the function is executed and may be out of date by the time you examine it. Note, however, that some flag values cannot be changed and are therefore permanently reliable. See SecCodeStatus for a list of possible values.

Specify the kSecCSDynamicInformation flag when calling the SecCodeCopySigningInformation(_:_:_:) function to get this information.

