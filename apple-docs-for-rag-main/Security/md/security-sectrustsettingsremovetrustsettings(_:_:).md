

- Security
-  SecTrustSettingsRemoveTrustSettings(\_:\_:) 

Function

# SecTrustSettingsRemoveTrustSettings(\_:\_:)

Deletes the trust settings for a certificate.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTrustSettingsRemoveTrustSettings(
    _ certRef: SecCertificate,
    _ domain: SecTrustSettingsDomain
) -> OSStatus
```

## Parameters 

`certRef`  

The certificate whose trust settings you wish to remove. Pass the value kSecTrustSettingsDefaultRootCertSetting to remove the default root certificate trust settings for the domain.

`domain`  

The trust settings domain for which you wish to remove the trust settings. For possible values, see SecTrustSettingsDomain.

## Return Value

A result code. See Security Framework Result Codes. Returns errSecItemNotFound if no trust settings exist for the certificate.

## Discussion

If a certificate has no trust settings, the certificate must be verified to a known, trusted certificate.

