

- Network
- NWProtocolIP
-  NWProtocolIP.Options 

Class

# NWProtocolIP.Options

A container of options for configuring how IP is used on a connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class Options
```

## Topics

### Selecting an IP Version

var version: NWProtocolIP.Options.Version

A required IP version that disables all other versions for a connection.

enum Version

IP versions to require on connections and listeners.

### Customizing IP Behavior

var shouldCalculateReceiveTime: Bool

A Boolean that indicates whether a connection delivers receive timestamps for IP packets.

var hopLimit: UInt8

The default hop limit for packets a connection generates.

var useMinimumMTU: Bool

A Boolean indicating that the connection uses the minimum MTU value, which is 1280 bytes for IPv6.

var disableFragmentation: Bool

A Boolean that indicates whether fragmentation is disabled on outbound packets.

### Instance Properties

var disableMulticastLoopback: Bool

var localAddressPreference: NWProtocolIP.Options.AddressPreference

### Enumerations

enum AddressPreference

## Relationships

### Inherits From

- NWProtocolOptions

### Conforms To

- Sendable

## See Also

### Configuring IP Connections

static let definition: NWProtocolDefinition

The system definition of the Internet Protocol.

