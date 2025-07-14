

- Security
-  SecCertificateCopySerialNumber(\_:) Deprecated

Function

# SecCertificateCopySerialNumber(\_:)

Returns a copy of a certificate’s serial number.

iOS 10.3–11.0DeprecatediPadOS 10.3–11.0DeprecatedmacOS 10.7–10.13DeprecatedtvOS 10.2–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.2–4.0Deprecated

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
func SecCertificateCopySerialNumber(_ certificate: SecCertificate) -> CFData?
```

**macOS**

``` source
func SecCertificateCopySerialNumber(
    _ certificate: SecCertificate,
    _ error: UnsafeMutablePointer?>?
) -> CFData?
```

Deprecated

Use SecCertificateCopySerialNumberData(_:_:) instead.

## Parameters 

`certificate`  

The certificate from which the serial number should be copied.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

A data instance containing a DER-encoded integer for the certificate’s serial number (without the tag and length fields) or `nil` if an error occurred. In Objective-C, free this object with a call to CFRelease when you are done with it.

