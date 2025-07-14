

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBHIDDescriptor 

Type Alias

# IOUSBHIDDescriptor

A structure that defines the USB HID descriptor.

macOS 10.0+

``` source
typedef struct IOUSBHIDDescriptor IOUSBHIDDescriptor;
```

## Discussion

See the USB Implementers Forum (USB-IF) *Device Class Definition for Human Interface Devices (HID)* for more information.

## Topics

### Getting the Properties

descLen

The size of the descriptor.

descType

The type of the descriptor.

descVersNum

The verison number of the descriptor.

hidCountryCode

The country or region code of the localized hardware.

hidDescriptorLengthHi

The high byte length of the descriptor.

hidDescriptorLengthLo

The low byte length of the descriptor.

hidDescriptorType

The class type of the descriptor.

hidNumDescriptors

The number of class descriptors.

## See Also

### HID Descriptors

IOUSBHIDData

Data related to the mouse and keyboard.

IOUSBHIDDataPtr

A pointer to a structure related to mouse and keyboard data.

IOUSBHIDDescriptorPtr

A pointer to a structure that defines the USB HID descriptor.

IOUSBHIDReportDesc

A structure that defines the USB HID report descriptor header.

IOUSBHIDReportDescPtr

A pointer to a structure that defines the USB HID report descriptor header.

### Related Documentation

IOUSBHIDDescriptor

