

- Security
-  SecTrustSetAnchorCertificatesOnly(\_:\_:) 

Function

# SecTrustSetAnchorCertificatesOnly(\_:\_:)

Reenables trusting built-in anchor certificates.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustSetAnchorCertificatesOnly(
    _ trust: SecTrust,
    _ anchorCertificatesOnly: Bool
) -> OSStatus
```

## Parameters 

`trust`  

The trust management object containing the certificate you want to evaluate. A trust management object includes the certificate to be verified plus the policy or policies to be used in evaluating trust. It can optionally also include other certificates to be used in verifying the first certificate. Use the SecTrustCreateWithCertificates(_:_:_:) function to create a trust management object.

`anchorCertificatesOnly`  

If `true`, disables trusting any anchors other than the ones passed in with the SecTrustSetAnchorCertificates(_:_:) function.  If `false`, the built-in anchor certificates are also trusted. If SecTrustSetAnchorCertificates(_:_:) is called and SecTrustSetAnchorCertificatesOnly(_:_:) is not called, only the anchors explicitly passed in are trusted.

## Return Value

A result code. See Security Framework Result Codes.

## Mentioned in 

Configuring a Trust

## Discussion

It is safe to call this function concurrently on two or more threads as long as it is not used to change the value of a trust management object that is simultaneously being used by another function. For example, you cannot call this function on one thread at the same time as you are calling the SecTrustEvaluateWithError(_:_:) function for the same trust management object on another thread, but you can call this function and simultaneously evaluate a different trust management object on another thread. Similarly, calls to functions that return information about a trust management object (such as the SecTrustCopyCustomAnchorCertificates(_:_:) function) may fail or return an unexpected result if this function is simultaneously changing the same trust management object on another thread.

## See Also

### Related Documentation

func SecTrustCopyCustomAnchorCertificates(SecTrust, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the custom anchor certificates, if any, used by a given trust.

func SecTrustCopyAnchorCertificates(UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the anchor (root) certificates stored by macOS.

