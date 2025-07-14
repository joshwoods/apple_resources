

- Security
-  SecTrustSettingsCopyCertificates(\_:\_:) 

Function

# SecTrustSettingsCopyCertificates(\_:\_:)

Obtains an array of all certificates that have trust settings in a specific trust settings domain.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTrustSettingsCopyCertificates(
    _ domain: SecTrustSettingsDomain,
    _ certArray: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`domain`  

The trust settings domain for which you want a list of certificates. For possible values, see SecTrustSettingsDomain.

`certArray`  

On return, an array of `SecCertificateRef` objects representing the certificates that have trust settings in the specified domain. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes. Returns errSecNoTrustSettings if no trust settings exist for the specified domain.

