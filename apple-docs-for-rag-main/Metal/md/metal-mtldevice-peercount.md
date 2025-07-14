

- Metal
- MTLDevice
-  peerCount 

Instance Property

# peerCount

The total number of GPUs in the peer group, if applicable.

macOS 10.15+

``` source
var peerCount: UInt32 { get }
```

**Required**

## Discussion

A peer count value of `0` indicates the GPU isn’t in a peer group. Otherwise, the GPU is in a peer group and the value represents the total number of GPUs in the group, including this one.

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

var peerGroupID: UInt64

The peer group ID the GPU belongs to, if applicable.

**Required**

var peerIndex: UInt32

The unique identifier for a GPU in a peer group.

**Required**

