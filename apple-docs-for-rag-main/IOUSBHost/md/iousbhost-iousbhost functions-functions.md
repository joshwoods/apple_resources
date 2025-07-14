

- IOUSBHost
-  IOUSBHost Functions 

API Collection

# IOUSBHost Functions

## Topics

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

func IOUSBHostCILinkStateToString(IOUSBHostCILinkState) -> UnsafePointer&lt;CChar>!

func IOUSBHostCIMessageStatusFromIOReturn(IOReturn) -> IOUSBHostCIMessageStatus

func IOUSBHostCIMessageStatusToIOReturn(IOUSBHostCIMessageStatus) -> IOReturn

func IOUSBHostCIMessageStatusToString(IOUSBHostCIMessageStatus) -> UnsafePointer&lt;CChar>!

func IOUSBHostCIMessageTypeToString(IOUSBHostCIMessageType) -> UnsafePointer&lt;CChar>!

func IOUSBHostCIPortStateToString(IOUSBHostCIPortState) -> UnsafePointer&lt;CChar>!

## See Also

### Reference

IOUSBHost Structures

IOUSBHost Enumerations

IOUSBHost Constants

IOUSBHost Data Types

