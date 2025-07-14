

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  markFailed(error:) 

Instance Method

# markFailed(error:)

Indicates to a connection that your protocol has encountered an error, or has gracefully closed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func markFailed(error: NWError?)
```

## See Also

### Managing Instance Lifetime

func markReady()

Indicates to a connection that your protocol’s handshake is complete.

func prependApplicationProtocol(options: NWProtocolOptions) throws

Dynamically adds another protocol that will run above your protocol after your protocol calls markReady().

