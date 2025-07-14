

- IOUSBHost
- IOUSBHostObject
-  Parsing USB Descriptors 

API Collection

# Parsing USB Descriptors

Extract information from various USB descriptors using helper methods.

## Topics

### Configuration Descriptor Parsing

func IOUSBGetNextDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next descriptor in a configuration descriptor.

func IOUSBGetNextDescriptorWithType(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next descriptor in a configuration descriptor that matches the type.

func IOUSBGetNextAssociatedDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next associated descriptor in a configuration descriptor.

func IOUSBGetNextAssociatedDescriptorWithType(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next associated descriptor in a configuration descriptor and matches the type.

func IOUSBGetNextInterfaceAssociationDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBInterfaceAssociationDescriptor>!

Obtains the next interface association descriptor in a configuration descriptor.

func IOUSBGetNextInterfaceDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBInterfaceDescriptor>!

Obtains the next interface descriptor in a configuration descriptor.

func IOUSBGetConfigurationMaxPowerMilliAmps(UInt32, UnsafePointer&lt;IOUSBConfigurationDescriptor>!) -> UInt32

Obtains the maximum bus current that a configuration descriptor requires.

### BOS Descriptor Parsing

func IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityUSB2Extension>!

Obtains the first USB 2.0 extension capability descriptor in a BOS descriptor.

func IOUSBGetNextCapabilityDescriptorWithType(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!

Obtains the next descriptor matching a specific type within a BOS descriptor.

func IOUSBGetNextCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!

Obtains the next device capability descriptor in a BOS descriptor.

func IOUSBGetSuperSpeedDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilitySuperSpeedUSB>!

Obtains the first SuperSpeed capability descriptor in a BOS descriptor.

func IOUSBGetContainerIDDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityContainerID>!

Obtains the first container ID capability descriptor in a BOS descriptor.

func IOUSBGetBillboardDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityBillboard>!

Obtains the first billboard capability descriptor in a BOS descriptor.

### Endpoint Descriptor Parsing

func IOUSBGetNextEndpointDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBInterfaceDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBEndpointDescriptor>!

Obtains the next endpoint descriptor for an interface descriptor.

func IOUSBGetEndpointDirection(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

Obtains the direction of an endpoint from an endpoint descriptor.

func IOUSBGetEndpointAddress(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

Obtains the direction and number of an endpoint from an endpoint descriptor.

func IOUSBGetEndpointNumber(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

Obtains the number of an endpoint from an endpoint descriptor.

func IOUSBGetEndpointType(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

Obtains the type of an endpoint from an endpoint descriptor.

func IOUSBGetEndpointMaxPacketSize(UInt32, UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt16

Obtains the maximum packet size from an endpoint descriptor.

func IOUSBGetEndpointIntervalEncodedMicroframes(UInt32, UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt32

Obtains the interval of an endpoint descriptor.

func IOUSBGetEndpointIntervalMicroframes(UInt32, UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt32

Obtains the interval of an endpoint descriptor.

func IOUSBGetEndpointIntervalFrames(UInt32, UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt32

Obtains the interval of an endpoint descriptor.

func IOUSBGetEndpointMaxStreamsEncoded(UInt32, UnsafePointer&lt;IOUSBEndpointDescriptor>!, UnsafePointer&lt;IOUSBSuperSpeedEndpointCompanionDescriptor>!) -> UInt32

Obtains the number of streams that an endpoint supports.

func IOUSBGetEndpointMaxStreams(UInt32, UnsafePointer&lt;IOUSBEndpointDescriptor>!, UnsafePointer&lt;IOUSBSuperSpeedEndpointCompanionDescriptor>!) -> UInt32

Obtains the number of supported streams.

## See Also

### Retrieving Base Class Descriptors

