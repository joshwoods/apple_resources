

- Metal
- MTLDevice
-  peerGroupID 

Instance Property

# peerGroupID

The peer group ID the GPU belongs to, if applicable.

macOS 10.15+

``` source
var peerGroupID: UInt64 { get }
```

**Required**

## Mentioned in 

Transferring Data Between Connected GPUs

## Discussion

A group ID value of `0` indicates the GPU isn’t in a peer group. Otherwise, the GPU is in a peer group and the value is the group’s ID. All other GPUs in the same peer group have the same group ID.

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

enum MTLDeviceLocation

Indicates the location of the GPU relative to the system it’s connect to.

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

var peerCount: UInt32

The total number of GPUs in the peer group, if applicable.

**Required**

var peerIndex: UInt32

The unique identifier for a GPU in a peer group.

**Required**

