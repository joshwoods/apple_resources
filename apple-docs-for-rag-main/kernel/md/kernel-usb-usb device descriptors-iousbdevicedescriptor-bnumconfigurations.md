

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDeviceDescriptor
-  bNumConfigurations 

Instance Property

# bNumConfigurations

The number of configurations that the device supports.

macOS 10.0+

``` source
uint8_t bNumConfigurations;
```

## See Also

### Getting the Device Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bcdUSB

The USB specification version number that the device is compliant with.

bDeviceClass

The class code indicating the behavior of this device.

bDeviceSubClass

The subclass code that further defines the behavior of this device.

bDeviceProtocol

The protocol that the device supports.

bMaxPacketSize0

An exponent value that specifies the maximum packet size for endpoint `0`.

idVendor

The ID of the device’s manufacturer.

idProduct

The product ID that the manufacturer assigns.

bcdDevice

The device release number as a binary-coded decimal.

iManufacturer

The index of the string descriptor that describes the manufacturer.

iProduct

The index of the string descriptor that describes the product.

iSerialNumber

The index of the string descriptor that describes the device’s serial number.

