

- Security
-  SecTrustEvaluateAsync(\_:\_:\_:) Deprecated

Function

# SecTrustEvaluateAsync(\_:\_:\_:)

Evaluates a trust object asynchronously on the specified dispatch queue.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15DeprecatedtvOS 7.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–6.0Deprecated

``` source
func SecTrustEvaluateAsync(
    _ trust: SecTrust,
    _ queue: dispatch_queue_t?,
    _ result: @escaping SecTrustCallback
) -> OSStatus
```

Deprecated

Use SecTrustEvaluateAsyncWithError(_:_:_:) instead.

## Parameters 

`trust`  

The trust management object to evaluate. A trust management object includes the certificate to be verified plus the policy or policies to be used in evaluating trust. It can optionally also include other certificates to be used in verifying the first certificate. Use the SecTrustCreateWithCertificates(_:_:_:) function to create a trust management object.

`queue`  

The dispatch queue on which the result block should execute.

`result`  

A block called with the result of evaluation. See SecTrustResultType for descriptions of possible values.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This function is functionally equivalent to SecTrustEvaluate(_:_:) except that it performs evaluation asynchronously and calls a block when evaluation completes. For a detailed discussion of the evaluation process, see SecTrustEvaluate(_:_:).

