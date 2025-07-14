

- Security
-  SecTrustSetSignedCertificateTimestamps(\_:\_:) 

Function

# SecTrustSetSignedCertificateTimestamps(\_:\_:)

Attaches signed certificate timestamp data to a trust object.

iOS 12.1.1+iPadOS 12.1.1+Mac Catalyst 13.1+macOS 10.14.2+tvOS 12.1.1+visionOS 1.0+watchOS 5.1.1+

``` source
func SecTrustSetSignedCertificateTimestamps(
    _ trust: SecTrust,
    _ sctArray: CFArray?
) -> OSStatus
```

## Parameters 

`trust`  

The trust object to which the timestamp data should be attached.

`sctArray`  

An array of CFData instances, each of which contains a signed certificate timestamp.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Use this function to provide secure certificate timestamps, which might be obtained during a TLS/SSL handshake, as input to a trust evaluation. For more information, see RFC 6962.

