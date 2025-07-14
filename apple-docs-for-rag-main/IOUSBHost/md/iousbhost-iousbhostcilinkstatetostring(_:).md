

- IOUSBHost
-  IOUSBHostCILinkStateToString(\_:) 

Function

# IOUSBHostCILinkStateToString(\_:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBHostCILinkStateToString(_ linkState: IOUSBHostCILinkState) -> UnsafePointer!
```

## See Also

### Functions

func IOUSBGetEndpointBurstSize(UInt32, UnsafePointer&lt;IOUSBEndpointDescriptor>!, UnsafePointer&lt;IOUSBSuperSpeedEndpointCompanionDescriptor>!, UnsafePointer&lt;IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor>!) -> UInt32

func IOUSBGetEndpointMult(UInt32, UnsafePointer&lt;IOUSBEndpointDescriptor>!, UnsafePointer&lt;IOUSBSuperSpeedEndpointCompanionDescriptor>!, UnsafePointer&lt;IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor>!) -> UInt8

func IOUSBGetEndpointSynchronizationType(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

func IOUSBGetEndpointUsageType(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

func IOUSBGetPlatformCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBPlatformCapabilityDescriptor>!

func IOUSBGetPlatformCapabilityDescriptorWithUUID(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafeMutablePointer&lt;UInt8>!) -> UnsafePointer&lt;IOUSBPlatformCapabilityDescriptor>!

func IOUSBGetSuperSpeedPlusDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilitySuperSpeedPlusUSB>!

func IOUSBHostCIControllerStateToString(IOUSBHostCIControllerState) -> UnsafePointer&lt;CChar>!

func IOUSBHostCIDeviceSpeedToString(IOUSBHostCIDeviceSpeed) -> UnsafePointer&lt;CChar>!

func IOUSBHostCIDeviceStateToString(IOUSBHostCIDeviceState) -> UnsafePointer&lt;CChar>!

func IOUSBHostCIEndpointStateToString(IOUSBHostCIEndpointState) -> UnsafePointer&lt;CChar>!

func IOUSBHostCIExceptionTypeToString(IOUSBHostCIExceptionType) -> UnsafePointer&lt;CChar>!

func IOUSBHostCILinkStateEnabled(IOUSBHostCILinkState) -> Bool

func IOUSBHostCIMessageStatusFromIOReturn(IOReturn) -> IOUSBHostCIMessageStatus

func IOUSBHostCIMessageStatusToIOReturn(IOUSBHostCIMessageStatus) -> IOReturn

