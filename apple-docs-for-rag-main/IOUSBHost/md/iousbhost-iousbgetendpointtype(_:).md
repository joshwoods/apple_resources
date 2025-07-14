

- IOUSBHost
-  IOUSBGetEndpointType(\_:) 

Function

# IOUSBGetEndpointType(\_:)

Obtains the type of an endpoint from an endpoint descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetEndpointType(_ descriptor: UnsafePointer!) -> UInt8
```

## Parameters 

`descriptor`  

An endpoint descriptor to parse.

## Return Value

The type found.

## See Also

### Endpoint Descriptor Parsing

func IOUSBGetNextEndpointDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBInterfaceDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBEndpointDescriptor>!

Obtains the next endpoint descriptor for an interface descriptor.

func IOUSBGetEndpointDirection(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

Obtains the direction of an endpoint from an endpoint descriptor.

func IOUSBGetEndpointAddress(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

Obtains the direction and number of an endpoint from an endpoint descriptor.

func IOUSBGetEndpointNumber(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

Obtains the number of an endpoint from an endpoint descriptor.

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

