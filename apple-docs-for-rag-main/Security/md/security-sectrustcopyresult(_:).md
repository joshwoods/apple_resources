

- Security
-  SecTrustCopyResult(\_:) 

Function

# SecTrustCopyResult(\_:)

Returns a dictionary containing information about an evaluated trust.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustCopyResult(_ trust: SecTrust) -> CFDictionary?
```

## Parameters 

`trust`  

The evaluated trust.

## Return Value

A dictionary containing keys with values that describe the result of the trust evaluation, or `NULL` when no information is available or if the trust has not been evaluated. See Trust Result Dictionary Keys for the list of possible keys. In Objective-C, use CFRelease to free the dictionary’s memory when you are done with it.

## Discussion

Call one of the SecTrustEvaluateWithError(_:_:) or SecTrustEvaluateAsyncWithError(_:_:_:) methods before calling SecTrustCopyResult(_:).

