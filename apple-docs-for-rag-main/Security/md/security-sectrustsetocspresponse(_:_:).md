

- Security
-  SecTrustSetOCSPResponse(\_:\_:) 

Function

# SecTrustSetOCSPResponse(\_:\_:)

Attaches Online Certificate Status Protocol (OSCP) response data to a trust object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustSetOCSPResponse(
    _ trust: SecTrust,
    _ responseData: CFTypeRef?
) -> OSStatus
```

## Parameters 

`trust`  

The trust evaluation object to modify.

`responseData`  

Either a CFData object containing a single DER-encoded OCSPResponse (per RFC2560), or a CFArray of these.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function allows the caller to provide OCSPResponse data (which may be obtained during a TLS/SSL handshake, per RFC3546) as input to a trust evaluation. If this data is available, it can obviate the need to contact an OCSP server for current revocation information.

