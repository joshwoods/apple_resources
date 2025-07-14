

- Security
-  SecTrustCopyAnchorCertificates(\_:) 

Function

# SecTrustCopyAnchorCertificates(\_:)

Retrieves the anchor (root) certificates stored by macOS.

macOS 10.3+

``` source
func SecTrustCopyAnchorCertificates(_ anchors: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`anchors`  

On return, points to an array of certificate objects for trusted anchor (root) certificates, which is the default set of anchors for the caller. In Objective-C, call the CFRelease function to release the CFArray object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function retrieves the certificates in the system’s store of anchor certificates (see SecTrustSetAnchorCertificates(_:_:)). You can use the SecCertificate objects retrieved by this function as input to other functions of this API, such as SecTrustCreateWithCertificates(_:_:_:).

It is safe to call this function concurrently on two or more threads as long as it is not used to get values from a trust management object that is simultaneously being changed by another function. For example, you can call this function on two threads at the same time, but not if you are simultaneously calling the SecTrustSetAnchorCertificates(_:_:) function for the same trust management object on another thread.

## See Also

### Related Documentation

func SecTrustSetAnchorCertificates(SecTrust, CFArray?) -> OSStatus

Sets the anchor certificates used when evaluating a trust management object.

