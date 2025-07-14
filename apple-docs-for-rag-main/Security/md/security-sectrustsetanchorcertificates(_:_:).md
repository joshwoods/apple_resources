

- Security
-  SecTrustSetAnchorCertificates(\_:\_:) 

Function

# SecTrustSetAnchorCertificates(\_:\_:)

Sets the anchor certificates used when evaluating a trust management object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustSetAnchorCertificates(
    _ trust: SecTrust,
    _ anchorCertificates: CFArray?
) -> OSStatus
```

## Parameters 

`trust`  

The trust management object containing the certificate you want to evaluate. A trust management object includes the certificate to be verified plus the policy or policies to be used in evaluating trust. It can optionally also include other certificates to be used in verifying the first certificate. Use the SecTrustCreateWithCertificates(_:_:_:) function to create a trust management object.

`anchorCertificates`  

A reference to an array of `SecCertificateRef` objects representing the set of anchor certificates that are to be considered valid (trusted) anchors by the SecTrustEvaluate(_:_:) function when verifying a certificate. Pass `NULL` to restore the default set of anchor certificates.

## Return Value

A result code. See Security Framework Result Codes.

## Mentioned in 

Configuring a Trust

## Discussion

The SecTrustEvaluateWithError(_:_:) function looks for an anchor certificate in the array of certificates specified by the SecTrustSetAnchorCertificates(_:_:) function, or uses a default set provided by the system. In OS X 10.3, for example, the default set of anchors was in the keychain file /System/Library/Keychains/X509Anchors. If you want to create a set of anchor certificates by modifying the default set, call the SecTrustCopyAnchorCertificates(_:) function to obtain the current set of anchor certificates, modify that set as you wish, and create a new array of certificates. Then call SecTrustSetAnchorCertificates(_:_:) with the modified array.

The list of custom anchor certificates is stored in the trust management object and can be retrieved with the SecTrustCopyCustomAnchorCertificates(_:_:) function.

Note that when you call the SecTrustSetAnchorCertificates(_:_:) function, you are effectively telling the evaluation function to use the anchor certificates in the specified array to evaluate trust regardless of any user-specified trust settings for those certificates. Furthermore, any intermediate certificates based on those anchor certificates are also trusted without consulting user trust settings.

Use the SecTrustSetKeychains(_:_:) function to set the keychains searched for intermediate certificates in the certificate chain.

It is safe to call this function concurrently on two or more threads as long as it is not used to change the value of a trust management object that is simultaneously being used by another function. For example, you cannot call this function on one thread at the same time as you are calling the evaluation function for the same trust management object on another thread, but you can call this function and simultaneously evaluate a different trust management object on another thread. Similarly, calls to functions that return information about a trust management object (such as the SecTrustCopyCustomAnchorCertificates(_:_:) function) may fail or return an unexpected result if this function is simultaneously changing the same trust management object on another thread.

Important

Calling this function without also calling SecTrustSetAnchorCertificatesOnly(_:_:) disables the trusting of any anchors other than the ones specified by this function call.

## See Also

### Related Documentation

func SecTrustCopyCustomAnchorCertificates(SecTrust, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the custom anchor certificates, if any, used by a given trust.

func SecTrustCopyAnchorCertificates(UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the anchor (root) certificates stored by macOS.

