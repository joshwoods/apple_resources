

- USBDriverKit
- IOUSBDeviceDescriptor
-  iManufacturer 

Instance Property

# iManufacturer

The index of the string descriptor that describes the manufacturer.

DriverKit 19.0+

``` source
uint8_t iManufacturer;
```

## See Also

### Getting the Device Properties

bLength

The length of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

bcdUSB

The USB specification release number with which the device complies.

bDeviceClass

The class code indicating the behavior of this device.

bDeviceSubClass

The subclass code that further defines the behavior of this device.

bDeviceProtocol

The protocol that the device supports.

bMaxPacketSize0

The maximum packet size for endpoint `0`, specified as an exponent value.

idVendor

The ID of the device’s manufacturer.

idProduct

The product ID assigned by the manufacturer.

bcdDevice

The release number of the device, specified as a binary-coded decimal number.

iProduct

The index of the string descriptor that describes the product.

iSerialNumber

The index of the string descriptor that describes the device’s serial number.

bNumConfigurations

The number of configurations that the device supports.

