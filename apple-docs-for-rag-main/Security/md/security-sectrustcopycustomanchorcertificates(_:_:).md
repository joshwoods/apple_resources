

- Security
-  SecTrustCopyCustomAnchorCertificates(\_:\_:) 

Function

# SecTrustCopyCustomAnchorCertificates(\_:\_:)

Retrieves the custom anchor certificates, if any, used by a given trust.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustCopyCustomAnchorCertificates(
    _ trust: SecTrust,
    _ anchors: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`trust`  

The trust management object from which you wish to retrieve the custom anchor certificates.

`anchors`  

On return, a reference to an array of `SecCertificateRef` objects representing the set of anchor certificates that are considered valid (trusted) anchors by the SecTrustEvaluateWithError(_:_:) function when verifying a certificate using the trust management object in the `trust` parameter. Returns `NULL` if no custom anchors have been specified. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

You can use the SecTrustSetAnchorCertificates(_:_:) function to set custom anchor certificates.

It is safe to call this function concurrently on two or more threads as long as it is not used to get values from a trust management object that is simultaneously being changed by another function. For example, you can call this function on two threads at the same time, but not if you are simultaneously calling the SecTrustSetAnchorCertificates(_:_:) function for the same trust management object on another thread.

## See Also

### Related Documentation

func SecTrustSetAnchorCertificates(SecTrust, CFArray?) -> OSStatus

Sets the anchor certificates used when evaluating a trust management object.

