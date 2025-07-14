

- Virtualization
- VZVirtioBlockDeviceConfiguration
-  init(attachment:) 

Initializer

# init(attachment:)

Creates a block device configuration object that uses the specified storage medium.

macOS 11.0+

``` source
init(attachment: VZStorageDeviceAttachment)
```

## Parameters 

`attachment`  

The attachment object that provides the storage for the device. For example, specify a VZDiskImageStorageDeviceAttachment object to implement the storage using a local disk image on the host computer.

## Return Value

A block storage device configuration object to include in your virtual machine’s configuration.

