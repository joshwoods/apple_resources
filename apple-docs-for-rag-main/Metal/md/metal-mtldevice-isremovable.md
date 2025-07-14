

- Metal
- MTLDevice
-  isRemovable 

Instance Property

# isRemovable

A Boolean value that indicates whether the GPU is removable.

Mac Catalyst 13.0+macOS 10.13+

``` source
var isRemovable: Bool { get }
```

**Required**

## Mentioned in 

Finding Multiple GPUs on an Intel-based Mac

## Discussion

You can respond to GPU removal notifications by registering with the MTLCopyAllDevicesWithObserver(handler:) function in Swift, or the MTLCopyAllDevicesWithObserver function in Objective-C, and responding to the removalRequested and wasRemoved device notification names.

Important

If a person removes a GPU without warning, MTLDevice APIs may fail even before your app receives a wasRemoved notification.

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

