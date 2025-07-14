

- Security
-  kSecCodeInfoRequirementData 

Global Variable

# kSecCodeInfoRequirementData

A key whose value is the internal requirements of the code as a binary blob.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoRequirementData: CFString
```

## Discussion

The value is a CFData object. If there is an explicit designated requirement, then it’s included in this data blob.

Specify the kSecCSRequirementInformation flag when calling the SecCodeCopySigningInformation(_:_:_:) function to get this information.

