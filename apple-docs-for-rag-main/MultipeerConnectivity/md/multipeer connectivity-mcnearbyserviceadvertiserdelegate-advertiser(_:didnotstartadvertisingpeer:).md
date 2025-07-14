

- Multipeer Connectivity
- MCNearbyServiceAdvertiserDelegate
-  advertiser(\_:didNotStartAdvertisingPeer:) 

Instance Method

# advertiser(\_:didNotStartAdvertisingPeer:)

Called when advertisement fails.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
optional func advertiser(
    _ advertiser: MCNearbyServiceAdvertiser,
    didNotStartAdvertisingPeer error: any Error
)
```

## Parameters 

`advertiser`  

The advertiser object that failed to begin advertising.

`error`  

An error object that indicates what went wrong.

