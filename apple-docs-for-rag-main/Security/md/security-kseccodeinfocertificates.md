

- Security
-  kSecCodeInfoCertificates 

Global Variable

# kSecCodeInfoCertificates

A key whose value is an array of certificates representing the certificate chain of the signing certificate as seen by the system.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoCertificates: CFString
```

## Discussion

The value is a CFArray array of SecCertificate objects that the system uses to process the signature. Absent for ad-hoc signed code. May be partial or absent in the case of error.

Specify the kSecCSSigningInformation flag when calling the SecCodeCopySigningInformation(_:_:_:) function to get this information.

