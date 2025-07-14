

- Security
-  SecTrustGetNetworkFetchAllowed(\_:\_:) 

Function

# SecTrustGetNetworkFetchAllowed(\_:\_:)

Indicates whether a trust evaluation is permitted to fetch missing intermediate certificates from the network.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustGetNetworkFetchAllowed(
    _ trust: SecTrust,
    _ allowFetch: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`trust`  

The trust evaluation object to query.

`allowFetch`  

A pointer to a Boolean that the function sets to true to indicate that the trust evaluation process is permitted to download missing certificates from the network, or false otherwise.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

By default, network fetch of missing certificates is enabled if the trust evaluation includes the SSL policy. Otherwise it is disabled.

