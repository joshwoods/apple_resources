

- Security
-  SecCertificateCopyNormalizedIssuerContent(\_:\_:) Deprecated

Function

# SecCertificateCopyNormalizedIssuerContent(\_:\_:)

Returns a normalized copy of the distinguished name (DN) of the issuer of a certificate.

macOS 10.7–10.12.4Deprecated

``` source
func SecCertificateCopyNormalizedIssuerContent(
    _ certificate: SecCertificate,
    _ error: UnsafeMutablePointer?>?
) -> CFData?
```

Deprecated

SecCertificateCopyNormalizedIssuerContent is deprecated. Use SecCertificateCopyNormalizedIssuerSequence instead.

## Parameters 

`certificate`  

The certificate from which the issuer’s distinguished name should be copied.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

A data object containing a DER-encoded X.509 distinguished name suitable for use with SecItemCopyMatching(_:_:). Returns `NULL` if an error occurred. In Objective-C, free the object with a call to the CFRelease function when you are done with it.

## Discussion

To obtain a copy of the issuer’s distinguished name in a format suitable for display purposes, call SecCertificateCopyValues(_:_:_:) instead.

