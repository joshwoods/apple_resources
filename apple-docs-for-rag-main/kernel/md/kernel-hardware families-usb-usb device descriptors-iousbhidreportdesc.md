

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBHIDReportDesc 

Type Alias

# IOUSBHIDReportDesc

A structure that defines the USB HID report descriptor header.

macOS 10.0+

``` source
typedef struct IOUSBHIDReportDesc IOUSBHIDReportDesc;
```

## Discussion

See the USB Implementers Forum (USB-IF) *Device Class Definition for Human Interface Devices (HID)* for more information.

## Topics

### Getting the Properties

hidDescriptorType

The type of the descriptor.

hidDescriptorLengthHi

The high byte length of the descriptor.

hidDescriptorLengthLo

The low byte length of the descriptor.

## See Also

### HID Descriptors

IOUSBHIDData

Data related to the mouse and keyboard.

IOUSBHIDDataPtr

A pointer to a structure related to mouse and keyboard data.

IOUSBHIDDescriptor

A structure that defines the USB HID descriptor.

IOUSBHIDDescriptorPtr

A pointer to a structure that defines the USB HID descriptor.

IOUSBHIDReportDescPtr

A pointer to a structure that defines the USB HID report descriptor header.

### Related Documentation

IOUSBHIDReportDesc

