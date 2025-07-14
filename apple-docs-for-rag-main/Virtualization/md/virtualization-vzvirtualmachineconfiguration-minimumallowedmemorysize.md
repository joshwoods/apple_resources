

- Virtualization
- VZVirtualMachineConfiguration
-  minimumAllowedMemorySize 

Type Property

# minimumAllowedMemorySize

The minimum amount of memory that you may configure for the VM.

macOS

``` source
class var minimumAllowedMemorySize: UInt64 { get }
```

## Discussion

The value in the memorySize property must be greater than or equal to the value in this property.

## See Also

### Sizing the memory partition

var memorySize: UInt64

The amount of physical memory the guest operating system recognizes.

class var maximumAllowedMemorySize: UInt64

The maximum amount of memory that you may configure for the VM.

var memoryBalloonDevices: [VZMemoryBalloonDeviceConfiguration]

An array that you configure with a memory balloon device, used to update the memory in the VM.

