

- Security
- SecTrustSettingsKeyUsage
-  useSignRevocation 

Type Property

# useSignRevocation

The key can be used to sign an OCSP (online certificate status protocol) message or CRL (certificate verification list), or to verify a signature.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var useSignRevocation: SecTrustSettingsKeyUsage { get }
```

## Discussion

OCSP messages and CRLs are used to revoke certificates.

