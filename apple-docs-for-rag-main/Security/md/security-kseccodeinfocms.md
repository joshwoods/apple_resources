

- Security
-  kSecCodeInfoCMS 

Global Variable

# kSecCodeInfoCMS

A key whose value is the CMS cryptographic object that secures the code signature.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoCMS: CFString
```

## Discussion

The value is a CFData object. Empty for ad-hoc signed code.

Specify the kSecCSSigningInformation flag when calling the SecCodeCopySigningInformation(_:_:_:) function to get this information.

