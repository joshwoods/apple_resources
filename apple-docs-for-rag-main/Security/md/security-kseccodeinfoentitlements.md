

- Security
-  kSecCodeInfoEntitlements 

Global Variable

# kSecCodeInfoEntitlements

A key whose value represents the embedded entitlement blob of the code, if any.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoEntitlements: CFString
```

## Discussion

The value is a CFData object.

Specify the kSecCSRequirementInformation flag when calling the SecCodeCopySigningInformation(_:_:_:) to get this information.

