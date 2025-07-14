

- Security
- SecTrustResultType
-  SecTrustResultType.recoverableTrustFailure 

Case

# SecTrustResultType.recoverableTrustFailure

Trust is denied, but recovery may be possible.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case recoverableTrustFailure
```

## Mentioned in 

Discovering Why a Trust Evaluation Failed

## Discussion

This value indicates that you should not trust the chain as is, but that the chain could be trusted with some minor change to the evaluation context, such as ignoring expired certificates or adding another anchor to the set of trusted anchors.

The way you handle this depends on the situation. For example, if you are performing signature validation and you know when the message was originally received, you should check again using that date to see if the message was valid when you originally received it.

You can also call the SecTrustCopyResult(_:) method to get more information about the results of the trust evaluation. If applicable, you can call one or more of the methods that start with `SecTrustSet` to correct or bypass the problem. Alternatively, in macOS, you can inform the user of the problem and call the SFCertificateTrustPanel class to let the user change the trust setting for the certificate.

After correcting the problem, reevaluate the trust. Each time you call SecTrustEvaluateWithError(_:_:) or SecTrustEvaluateAsyncWithError(_:_:_:), the method discards the results of any previous evaluation and replaces them with the new results.

You might receive the SecTrustResultType.recoverableTrustFailure value after an evaluation, but you can’t store the value as part of the user trust settings with a call to the SecTrustSettingsSetTrustSettings(_:_:_:) method.

