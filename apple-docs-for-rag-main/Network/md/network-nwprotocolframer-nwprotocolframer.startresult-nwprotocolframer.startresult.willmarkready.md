

- Network
- NWProtocolFramer
- NWProtocolFramer.StartResult
-  NWProtocolFramer.StartResult.willMarkReady 

Case

# NWProtocolFramer.StartResult.willMarkReady

The protocol will perform a handshake, preventing the overall connection from becoming ready until markReady() is called.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case willMarkReady
```

## See Also

### Related Documentation

func markReady()

Indicates to a connection that your protocol’s handshake is complete.

### Start Results

case ready

The protocol is immediately ready to send and receive data.

