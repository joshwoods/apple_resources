

- Security
-  kSecTrustSettingsAllowedError 

Global Variable

# kSecTrustSettingsAllowedError

A number which, if encountered during certificate verification, is ignored for that certificate.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kSecTrustSettingsAllowedError: String { get }
```

## Discussion

The value is a CFNumber object containing an `SInt32` value indicating a `CSSM_RETURN` result code.

