

- Security
-  SecCertificateCopyPublicKey(\_:) Deprecated

Function

# SecCertificateCopyPublicKey(\_:)

Retrieves the public key from a certificate.

iOS 10.3–12.0DeprecatediPadOS 10.3–12.0DeprecatedmacOS 10.3–10.14DeprecatedtvOS 10.2–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.2–5.0Deprecated

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
func SecCertificateCopyPublicKey(_ certificate: SecCertificate) -> SecKey?
```

**macOS**

``` source
func SecCertificateCopyPublicKey(
    _ certificate: SecCertificate,
    _ key: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

Use SecCertificateCopyKey(_:) instead.

## Parameters 

`certificate`  

The certificate object from which to retrieve the public key.

`key`  

In macOS, points to the public key for the specified certificate. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

In iOS, the certificate’s public key.

## Mentioned in 

Examining a Certificate

## Discussion

In macOS, a result code. See Security Framework Result Codes.

