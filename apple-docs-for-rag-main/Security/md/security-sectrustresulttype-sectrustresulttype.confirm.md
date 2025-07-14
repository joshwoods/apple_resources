

- Security
- SecTrustResultType
-  SecTrustResultType.confirm 

Case

# SecTrustResultType.confirm

User confirmation is required before proceeding.

tvOS 9.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
case confirm
```

## Discussion

This value indicates that the user previously chose to always be asked for permission before accepting one of the certificates in the chain. The Keychain Access utility refers to this value as “Ask Permission.” This return value is no longer used, but may occur in older versions of macOS.

Either ask the user what to do or reject the certificate. If you ask the user what to do in macOS, use an instance of the SFCertificateTrustPanel class.

