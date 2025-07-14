

- Metal
- MTLDevice
-  isLowPower 

Instance Property

# isLowPower

A Boolean value that indicates whether the GPU lowers its performance to conserve energy.

Mac Catalyst 13.0+macOS 10.11+

``` source
var isLowPower: Bool { get }
```

**Required**

## Mentioned in 

Finding Multiple GPUs on an Intel-based Mac

## Discussion

Some systems contain multiple GPUs that run with different performance and energy characteristics. At runtime, choose a GPU that best matches your performance needs while considering the current state of the system. For example, your app may choose a lower-power GPU if it doesn’t need the best possible performance on a MacBook Pro that’s running on battery power. For more information on discovering and selecting GPUs at runtime, see Multi-GPU Systems.

Note

Systems with Apple silicon only have one GPU, which removes the need to choose a GPU.

The property is typically true for integrated GPUs and false for discrete GPUs. However, an Apple silicon GPU on a Mac sets the property to false because it doesn’t need to lower its performance to conserve energy.

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

