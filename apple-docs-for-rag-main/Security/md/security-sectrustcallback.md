

- Security
-  SecTrustCallback 

Type Alias

# SecTrustCallback

A block called with the results of an asynchronous trust evaluation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias SecTrustCallback = (SecTrust, SecTrustResultType) -> Void
```

## Parameters 

`trustRef`  

The trust that was evaluated.

`trustResult`  

The result of the trust evaluation. See SecTrustResultType for a list of possible values.

## Discussion

Use a block of this type when making a call to SecTrustEvaluateAsync(_:_:_:) to receive the result of the trust evaluation.

