

- Security
-  SecTrustGetTrustResult(\_:\_:) 

Function

# SecTrustGetTrustResult(\_:\_:)

Returns the result code from the most recent trust evaluation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustGetTrustResult(
    _ trust: SecTrust,
    _ result: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`trust`  

The trust object from which results should be obtained

`result`  

A pointer that the function sets to point at a value that is the result type. See SecTrustResultType for possible values.

## Return Value

A result code. See Security Framework Result Codes.

## Mentioned in 

Discovering Why a Trust Evaluation Failed

## Discussion

If the trust object has not yet been evaluated, the result type is SecTrustResultType.invalid.

