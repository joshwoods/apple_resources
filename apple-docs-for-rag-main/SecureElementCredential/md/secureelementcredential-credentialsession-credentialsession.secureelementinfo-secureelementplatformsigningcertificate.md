

- SecureElementCredential
- CredentialSession
- CredentialSession.SecureElementInfo
-  secureElementPlatformSigningCertificate 

Instance Property

# secureElementPlatformSigningCertificate

A certificate you use to authenticate against the Certification Authority of the Secure Element hardware.

iOS 18.4+iPadOS 18.4+

``` source
let secureElementPlatformSigningCertificate: Data
```

## Discussion

This certificate contains Controlling Authority Security Domain public key information for authenticating a Secure Element Platform.

For more details, see the Mobile Secure Element specification from Apple Business Register.

## See Also

### Getting hardware information

let hardwareReleaseVersionInfo: String

A string that encodes the hardware and software release versions of the Secure Element.

