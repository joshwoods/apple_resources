

- Security
-  SecTrustCopyExceptions(\_:) 

Function

# SecTrustCopyExceptions(\_:)

Returns an opaque cookie containing exceptions to trust policies that will allow future evaluations of the current certificate to succeed.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustCopyExceptions(_ trust: SecTrust) -> CFData?
```

## Parameters 

`trust`  

The evaluated trust management object whose policies you wish to retrieve.

## Return Value

An opaque cookie. If you pass this cookie to SecTrustSetExceptions(_:_:), that function sets a list of exceptions for future processing of the certificate. Once this list of exceptions are set, a subsequent call to SecTrustEvaluateWithError(_:_:) for that certificate will return `true`.

## Discussion

Note: If a new error occurs that did not occur when this function was called originally, the subsequent call to SecTrustEvaluateWithError(_:_:) can still fail. For example, if the certificate expires between calling `SecTrustCopyExceptions` and SecTrustEvaluateWithError(_:_:), evaluation will fail.

## Discussion

Normally this API should only be called after asking the user how to proceed, and even then, only if the user explicitly tells your application to trust the current certificate chain in spite of the errors presented.

## See Also

### Related Documentation

func SecTrustSetPolicies(SecTrust, CFTypeRef) -> OSStatus

Sets the policies to use in an evaluation.

