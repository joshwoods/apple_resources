

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBBOSDescriptor 

Type Alias

# IOUSBBOSDescriptor

The structure for storing a binary object store (BOS) descriptor.

macOS 10.7+

``` source
typedef struct IOUSBBOSDescriptor IOUSBBOSDescriptor;
```

## Discussion

For more information about this descriptor type, see USB 3.2, 9.6.2.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

wTotalLength

The length of this descriptor and all of its subdescriptors.

bNumDeviceCaps

The number of separate device capability descriptors in the binary object store.

## See Also

### BOS Descriptors

IOUSBBOSDescriptorPtr

A pointer to a structure for storing a binary object store (BOS) descriptor.

### Related Documentation

IOUSBBOSDescriptor

