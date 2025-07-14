

- Metal
-  MTLDeviceLocation 

Enumeration

# MTLDeviceLocation

Indicates the location of the GPU relative to the system it’s connect to.

macOS 10.15+

``` source
enum MTLDeviceLocation
```

## Overview

Check the location of a GPU by checking the location property of its MTLDevice instance.

## Topics

### Determining the GPU’s Location

case builtIn

A location that indicates the GPU is permanently connected to the system internally.

case slot

A GPU location that indicates a person connected the GPU to a system’s internal slot.

case external

A GPU location that indicates a person connected the GPU to the system with an external interface, such as Thunderbolt.

case unspecified

A value that indicates the system can’t determine how the GPU connects to it.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying a GPU Device

var name: String

The full name of the GPU device.

**Required**

var architecture: MTLArchitecture

The architectural details of the GPU device.

**Required**

class MTLArchitecture

A class that contains the architectural details of a GPU device.

var registryID: UInt64

The GPU device’s registry identifier.

**Required**

var location: MTLDeviceLocation

The physical location of the GPU relative to the system.

**Required**

var locationNumber: Int

A specific GPU position based on its general location.

**Required**

var isLowPower: Bool

A Boolean value that indicates whether the GPU lowers its performance to conserve energy.

**Required**

var isRemovable: Bool

A Boolean value that indicates whether the GPU is removable.

**Required**

var isHeadless: Bool

A Boolean value that indicates whether a GPU device doesn’t have a connection to a display.

**Required**

var peerGroupID: UInt64

The peer group ID the GPU belongs to, if applicable.

**Required**

var peerCount: UInt32

The total number of GPUs in the peer group, if applicable.

**Required**

var peerIndex: UInt32

The unique identifier for a GPU in a peer group.

**Required**

