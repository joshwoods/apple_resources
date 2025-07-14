

- Foundation
- URLProtocol
-  requestIsCacheEquivalent(\_:to:) 

Type Method

# requestIsCacheEquivalent(\_:to:)

A Boolean value indicating whether two requests are equivalent for cache purposes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func requestIsCacheEquivalent(
    _ a: URLRequest,
    to b: URLRequest
) -> Bool
```

## Parameters 

`a`  

The request to compare with `bRequest`.

`b`  

The request to compare with `aRequest`.

## Return Value

true if `aRequest` and `bRequest` are equivalent for cache purposes, false otherwise.

## Discussion

Requests are considered equivalent for cache purposes if and only if they would be handled by the same protocol and that protocol declares them equivalent after performing implementation-specific checks.

The URLProtocol implementation of this method compares the URLs of the requests to determine if the requests should be considered equivalent. Subclasses can override this method to provide protocol-specific comparisons.

