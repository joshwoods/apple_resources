

- Virtualization
- VZVirtualMachineConfiguration
-  memoryBalloonDevices 

Instance Property

# memoryBalloonDevices

An array that you configure with a memory balloon device, used to update the memory in the VM.

macOS 11.0+

``` source
var memoryBalloonDevices: [VZMemoryBalloonDeviceConfiguration] { get set }
```

## Discussion

Use this property to request a memory balloon device from the VM. The VM initially reserves the amount of memory in the memorySize property for the guest operating system. A balloon memory device asks the guest system to return memory pages that it isn’t using to the VM. You might use the device to reclaim memory when the amount of free memory on the host system runs low.

The default value of this property is an empty array, which doesn’t result in the creation of a balloon memory device. To create a balloon memory device, add a single VZVirtioTraditionalMemoryBalloonDeviceConfiguration object to the array. In response, the VM creates a VZVirtioTraditionalMemoryBalloonDevice object and adds it to its memoryBalloonDevices property. Use that object to change the amount of memory reserved for the guest system.

## See Also

### Sizing the memory partition

var memorySize: UInt64

The amount of physical memory the guest operating system recognizes.

class var minimumAllowedMemorySize: UInt64

The minimum amount of memory that you may configure for the VM.

class var maximumAllowedMemorySize: UInt64

The maximum amount of memory that you may configure for the VM.

