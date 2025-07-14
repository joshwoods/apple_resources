

- Security
- SecTrustSettingsResult
-  SecTrustSettingsResult.trustRoot 

Case

# SecTrustSettingsResult.trustRoot

This root certificate is explicitly trusted.

Mac Catalyst 13.0+macOS 10.0+

``` source
case trustRoot
```

## Discussion

If the certificate is not a root (self-signed) certificate, the usage constraints dictionary is invalid.

