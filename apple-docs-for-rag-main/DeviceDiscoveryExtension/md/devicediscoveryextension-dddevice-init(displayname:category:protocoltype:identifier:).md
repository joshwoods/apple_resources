

- DeviceDiscoveryExtension
- DDDevice
-  init(displayName:category:protocolType:identifier:) 

Initializer

# init(displayName:category:protocolType:identifier:)

Creates an object that describes a discovered device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
init(
    displayName: String,
    category: DDDevice.Category,
    protocolType: UTType,
    identifier: String
)
```

## Parameters 

`displayName`  

A name for the device to display to the user.

`category`  

An option that determines the icon that the picker UI displays for the device.

`protocolType`  

A custom universal type that describes the device’s manner of communication with the extension.

`identifier`  

A unique identifier for the device.

## Discussion

As an example `identifier` for Bluetooth devices, your extension can use the device’s local name (see CBAdvertisementDataLocalNameKey).

