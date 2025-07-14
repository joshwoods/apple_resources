

- IOUSBHost
-  IOUSBGetNextEndpointDescriptor(\_:\_:\_:) 

Function

# IOUSBGetNextEndpointDescriptor(\_:\_:\_:)

Obtains the next endpoint descriptor for an interface descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetNextEndpointDescriptor(
    _ configurationDescriptor: UnsafePointer!,
    _ interfaceDescriptor: UnsafePointer!,
    _ currentDescriptor: UnsafePointer!
) -> UnsafePointer!
```

## Parameters 

`configurationDescriptor`  

A configuration descriptor that contains the descriptors to iterate through.

`interfaceDescriptor`  

An interface descriptor within the bounds of `configurationDescriptor`.

`currentDescriptor`  

A descriptor pointer within the bounds of `configurationDescriptor`, or `nil`.

## Return Value

A descriptor pointer, or `nil` if no matching descriptor returns.

## Discussion

This method uses IOUSBGetNextAssociatedDescriptorWithType(_:_:_:_:) to find the next endpoint descriptor for a specific interface descriptor.

## See Also

### Endpoint Descriptor Parsing

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

