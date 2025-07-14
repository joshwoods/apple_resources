

- Security
-  SecTrustCopyPublicKey(\_:) Deprecated

Function

# SecTrustCopyPublicKey(\_:)

Returns the public key for a leaf certificate after it has been evaluated.

iOS 2.0–14.0DeprecatediPadOS 2.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.7–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–7.0Deprecated

``` source
func SecTrustCopyPublicKey(_ trust: SecTrust) -> SecKey?
```

## Parameters 

`trust`  

The trust management object for the certificate that has been evaluated. Use the SecTrustCreateWithCertificates(_:_:_:) function to create a trust management object.

## Return Value

The leaf certificate’s public key, or `NULL` if it the public key could not be extracted (this can happen with DSA certificate chains if the parameters in the chain cannot be found). In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Mentioned in 

Getting an Existing Key

Evaluating a Trust and Parsing the Result

## Discussion

Call the SecTrustEvaluateWithError(_:_:) function before calling this function.

When you call this function, it attempts to return the public key of the leaf certificate, even if the trust evaluation was unsuccessful. Even if the trust evaluation was successful, this function might still return `NULL`—for example, if the leaf certificate’s key can’t be extracted for some reason.

