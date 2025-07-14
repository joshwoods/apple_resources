

- Security
-  SecTrustSettingsCreateExternalRepresentation(\_:\_:) 

Function

# SecTrustSettingsCreateExternalRepresentation(\_:\_:)

Obtains an external, portable representation of the specified domain’s trust settings.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTrustSettingsCreateExternalRepresentation(
    _ domain: SecTrustSettingsDomain,
    _ trustSettings: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`domain`  

The trust settings domain for which you want an external representation of trust settings. For possible values, see SecTrustSettingsDomain.

`trustSettings`  

An external representation of the domain’s trust settings. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes. Returns errSecNoTrustSettings if no trust settings exist for the specified domain.

## Discussion

Trust settings for a certificate are associated with the hash of the certificate. Whenever the system encounters a certificate with the hash value associated with the trust settings, it applies those trust settings to the certificate. This function allows you to export trust settings to a portable data format that can subsequently be imported on another machine. You can use this ability, for example, to clone trust settings to all the machines within an enterprise or university.

