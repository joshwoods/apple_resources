

- Security
-  SecTrustSetNetworkFetchAllowed(\_:\_:) 

Function

# SecTrustSetNetworkFetchAllowed(\_:\_:)

Specifies whether a trust evaluation is permitted to fetch missing intermediate certificates from the network.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustSetNetworkFetchAllowed(
    _ trust: SecTrust,
    _ allowFetch: Bool
) -> OSStatus
```

## Parameters 

`trust`  

The trust evaluation object to modify.

`allowFetch`  

If true, and a certificate’s issuer is not present in the trust reference but its network location is known, the evaluation is permitted to attempt to download it automatically. Pass false to disable network fetch for this trust evaluation.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

By default, network fetch of missing certificates is enabled if the trust evaluation includes the SSL policy. Otherwise it is disabled.

