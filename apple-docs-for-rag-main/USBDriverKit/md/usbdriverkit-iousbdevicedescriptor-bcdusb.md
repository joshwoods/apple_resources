

- USBDriverKit
- IOUSBDeviceDescriptor
-  bcdUSB 

Instance Property

# bcdUSB

The USB specification release number with which the device complies.

DriverKit 19.0+

``` source
uint16_t bcdUSB;
```

## Discussion

The value in this field is formatted as a binary-coded decimal number.

## See Also

### Getting the Device Properties

bLength

The length of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

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

iManufacturer

The index of the string descriptor that describes the manufacturer.

iProduct

The index of the string descriptor that describes the product.

iSerialNumber

The index of the string descriptor that describes the device’s serial number.

bNumConfigurations

The number of configurations that the device supports.

