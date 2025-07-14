

- Security
-  SecTrustSettingsImportExternalRepresentation(\_:\_:) 

Function

# SecTrustSettingsImportExternalRepresentation(\_:\_:)

Imports trust settings into a trust domain.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTrustSettingsImportExternalRepresentation(
    _ domain: SecTrustSettingsDomain,
    _ trustSettings: CFData
) -> OSStatus
```

## Parameters 

`domain`  

The trust settings domain into which you want to import trust settings. For possible values, see SecTrustSettingsDomain.

`trustSettings`  

An external representation of the trust settings (created by the SecTrustSettingsCreateExternalRepresentation(_:_:) function) that you want to import.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Trust settings for a certificate are associated with the hash of the certificate. Whenever the system encounters a certificate with the hash value associated with the trust settings, it applies those trust settings to the certificate. This function allows you to import trust settings in a portable data format that was exported from another machine. You can use this ability, for example, to clone trust settings to all the machines within an enterprise or university.

