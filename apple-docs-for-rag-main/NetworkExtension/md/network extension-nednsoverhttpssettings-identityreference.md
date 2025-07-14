

- Network Extension
- NEDNSOverHTTPSSettings
-  identityReference 

Instance Property

# identityReference

A persistent keychain reference to a keychain item containing the certificate and private key components of the DNS client credential.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+visionOS 1.0+

``` source
var identityReference: Data? { get set }
```

## Discussion

The keychain item must have the kSecClassIdentity class.

