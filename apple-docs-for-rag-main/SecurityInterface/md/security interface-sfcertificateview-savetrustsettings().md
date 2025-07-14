

- Security Interface
- SFCertificateView
-  saveTrustSettings() 

Instance Method

# saveTrustSettings()

Saves the user’s current trust settings for the displayed certificate.

macOS 10.3+

``` source
@MainActor
func saveTrustSettings()
```

## Discussion

If trust settings are not editable, this method effectively does nothing. You can use doc://com.apple.documentation/documentation/security/certificate_key_and_trust_services/trust/1805379-sectrustgetusertrust to subsequently retrieve the trust settings.

## Topics

### Related Documentation

func setEditableTrust(Bool)

Specifies whether the user can edit the certificate’s trust settings.

