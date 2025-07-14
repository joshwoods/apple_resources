

- IOUSBHost
-  IOUSBGetEndpointMaxPacketSize(\_:\_:) 

Function

# IOUSBGetEndpointMaxPacketSize(\_:\_:)

Obtains the maximum packet size from an endpoint descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetEndpointMaxPacketSize(
    _ usbDeviceSpeed: UInt32,
    _ descriptor: UnsafePointer!
) -> UInt16
```

## Parameters 

`usbDeviceSpeed`  

The operational speed of the device.

`descriptor`  

The endpoint descriptor to parse.

## Return Value

The maximum packet size in bytes.

## Discussion

This method parses an endpoint descriptor to determine its maximum packet size, which doesn’t include mult or burst factors.

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

func IOUSBGetEndpointType(UnsafePointer&lt;IOUSBEndpointDescriptor>!) -> UInt8

Obtains the type of an endpoint from an endpoint descriptor.

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

