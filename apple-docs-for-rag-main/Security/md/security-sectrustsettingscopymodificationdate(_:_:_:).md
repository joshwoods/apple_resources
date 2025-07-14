

- Security
-  SecTrustSettingsCopyModificationDate(\_:\_:\_:) 

Function

# SecTrustSettingsCopyModificationDate(\_:\_:\_:)

Obtains the date and time at which a certificate’s trust settings were last modified.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTrustSettingsCopyModificationDate(
    _ certRef: SecCertificate,
    _ domain: SecTrustSettingsDomain,
    _ modificationDate: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`certRef`  

The certificate for which you wish to obtain the modification time. Pass the value `kSecTrustSettingsDefaultRootCertSetting` to obtain the modification time for the default root certificate trust settings for the domain.

`domain`  

The trust settings domain of the trust settings for which you wish to obtain the modification time (it’s possible for a single certificate to have trust settings in more than one domain). For possible values, see SecTrustSettingsDomain.

`modificationDate`  

On return, the date and time at which the certificate’s trust settings were last modified. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes. Returns errSecItemNotFound if no trust settings exist for the specified certificate and domain.

