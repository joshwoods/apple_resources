

- Network
- NWProtocolFramer
- NWProtocolFramer.StartResult
-  NWProtocolFramer.StartResult.ready 

Case

# NWProtocolFramer.StartResult.ready

The protocol is immediately ready to send and receive data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case ready
```

## See Also

### Start Results

case willMarkReady

The protocol will perform a handshake, preventing the overall connection from becoming ready until markReady() is called.

