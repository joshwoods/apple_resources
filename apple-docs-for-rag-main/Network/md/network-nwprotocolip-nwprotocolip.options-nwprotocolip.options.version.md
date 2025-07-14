

- Network
- NWProtocolIP
- NWProtocolIP.Options
-  NWProtocolIP.Options.Version 

Enumeration

# NWProtocolIP.Options.Version

IP versions to require on connections and listeners.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum Version
```

## Topics

### Versions

case any

Allow any IP version.

case v4

Require IP version 4.

case v6

Require IP version 6.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Selecting an IP Version

var version: NWProtocolIP.Options.Version

A required IP version that disables all other versions for a connection.

