

- vmnet
- interface_event_t
-  VMNET_INTERFACE_PACKETS_AVAILABLE 

Type Property

# VMNET_INTERFACE_PACKETS_AVAILABLE

Mac Catalyst 13.0+macOS 10.10+

``` source
static var VMNET_INTERFACE_PACKETS_AVAILABLE: interface_event_t { get }
```

## Discussion

Event indicating packets are available to be read on the interface.

The `event` dictionary passed in the callback returns the estimated number of packets available to be read using the vmnet_estimated_packets_available_key key.

