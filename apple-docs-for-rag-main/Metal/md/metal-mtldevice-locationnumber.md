

- Metal
- MTLDevice
-  locationNumber 

Instance Property

# locationNumber

A specific GPU position based on its general location.

macOS 10.15+

``` source
var locationNumber: Int { get }
```

**Required**

## Discussion

The meaning of the location number depends on a device’s location property:

- For MTLDeviceLocation.builtIn, the location number is `0` for low-power GPUs (see isLowPower) and `1` for other GPUs.

- For MTLDeviceLocation.slot, the location number represents the slot.

- For MTLDeviceLocation.external, the location number represents the Thunderbolt port.

Note

It’s possible for multiple devices to share the same location and number. For example, a card in a slot may have multiple GPUs, or a person may connect multiple eGPUs to the same Thunderbolt port.

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

