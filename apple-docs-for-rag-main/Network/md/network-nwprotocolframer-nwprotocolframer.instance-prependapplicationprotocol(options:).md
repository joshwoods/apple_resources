

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  prependApplicationProtocol(options:) 

Instance Method

# prependApplicationProtocol(options:)

Dynamically adds another protocol that will run above your protocol after your protocol calls markReady().

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func prependApplicationProtocol(options: NWProtocolOptions) throws
```

## See Also

### Managing Instance Lifetime

func markReady()

Indicates to a connection that your protocol’s handshake is complete.

func markFailed(error: NWError?)

Indicates to a connection that your protocol has encountered an error, or has gracefully closed.

