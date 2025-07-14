

- Security
-  SecTrustEvaluateWithError(\_:\_:) 

Function

# SecTrustEvaluateWithError(\_:\_:)

Evaluates trust for the specified certificate and policies.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func SecTrustEvaluateWithError(
    _ trust: SecTrust,
    _ error: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`trust`  

The trust management object to evaluate. A trust management object includes the certificate to be verified plus the policy or policies to be used in evaluating trust. It can optionally also include other certificates to be used in verifying the first certificate. Use the SecTrustCreateWithCertificates(_:_:_:) function to create a trust management object.

`error`  

An error pointer the method uses to return an error when trust evaluation fails. Set to `nil` to ignore the error.

## Return Value

true if the certificate is trusted; otherwise, false.

## Discussion

This method evaluates a certificate’s validity to establish trust for a particular use—for example, in creating a digital signature or to establish a Secure Sockets Layer connection. The method validates a certificate by verifying its signature plus the signatures of the certificates in its certificate chain, up to the anchor certificate, according to the policy or policies included in the trust management object.

If the trust management instance lacks some of the certificates needed to verify the leaf certificate, SecTrustEvaluateWithError(_:_:) searches for certificates:

- In the user’s keychain.

- Among any certificates you previously provided by calling SecTrustSetAnchorCertificates(_:_:).

- In a system-provided set of keychains provided for this purpose.

- Over the network, if certain extensions are present in the certificate used to build the chain.

Note

Although this method searches the keychain for intermediate certificates, it does not search the keychain for anchor (root) certificates. To add an anchor certificate, you must call SecTrustSetAnchorCertificates(_:_:).

Before calling SecTrustEvaluateWithError(_:_:), you can optionally call any of the methods that start with `SecTrustSet` to manage the evaluation. For example, you can verify the validity of the certificates in a trust at a particular date and time, rather than using the current date and time, by first calling the SecTrustSetVerifyDate(_:_:) method.

The SecTrustEvaluateWithError(_:_:) method returns a pass or fail indicator and an error describing the reason for any failure. In the case of multiple certificate failures, the error contains a code from Security Framework Result Codes representing the most serious. The localized description indicates the certificate with the most serious problem and the type of error. The underlying error, located in the error’s userInfo dictionary as the value for the NSUnderlyingErrorKey key, contains a localized description of each certificate in the chain that had an error and all errors found with that certificate.

To find out if you can recover from a trust failure, call the SecTrustGetTrustResult(_:_:) method. See the SecTrustResultType constants to learn how to interpret the value returned by that call.

Don’t call SecTrustEvaluateWithError(_:_:) from your app’s main run loop because it might require network access to fetch intermediate certificates, or to perform revocation checking. To perform evaluation asynchronously, use SecTrustEvaluateAsyncWithError(_:_:_:) instead.

