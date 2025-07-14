

- Security
-  SecTrustSetExceptions(\_:\_:) 

Function

# SecTrustSetExceptions(\_:\_:)

Sets a list of exceptions that should be ignored when the certificate is evaluated.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustSetExceptions(
    _ trust: SecTrust,
    _ exceptions: CFData?
) -> Bool
```

## Parameters 

`trust`  

The trust management object whose exception list you wish to modify.

`exceptions`  

An opaque cookie returned by a prior call to SecTrustCopyExceptions(_:).

## Return Value

A Boolean that is true if the exceptions cookies was valid and matches the current leaf certificate, false otherwise.

## Discussion

Important

Even if this function returns true, you must still call SecTrustEvaluateWithError(_:_:) because the evaluation can still fail if something changes between the initial evaluation and the reevaluation.

