

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  markReady() 

Instance Method

# markReady()

Indicates to a connection that your protocol’s handshake is complete.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func markReady()
```

## See Also

### Related Documentation

case willMarkReady

The protocol will perform a handshake, preventing the overall connection from becoming ready until markReady() is called.

### Managing Instance Lifetime

func markFailed(error: NWError?)

Indicates to a connection that your protocol has encountered an error, or has gracefully closed.

func prependApplicationProtocol(options: NWProtocolOptions) throws

Dynamically adds another protocol that will run above your protocol after your protocol calls markReady().

