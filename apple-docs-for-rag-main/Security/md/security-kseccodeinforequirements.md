

- Security
-  kSecCodeInfoRequirements 

Global Variable

# kSecCodeInfoRequirements

A key whose value is the internal requirements of the code as a text string in canonical syntax.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoRequirements: CFString
```

## Discussion

The value is a CFString object. If there is an explicit designated requirement, then it’s included in this text string.

Specify the kSecCSRequirementInformation flag when calling the SecCodeCopySigningInformation(_:_:_:) function to get this information.

