

- Core Media I/O
-  Overriding the default USB video class extension 

Article

# Overriding the default USB video class extension

Create a simple DriverKit extension to override the default driver-matching behavior for USB devices.

## Overview

Starting in macOS 12.3, the operating system provides a class-compliant Core Media I/O (CMIO) extension that enables the use of USB cameras and other video capture devices. When you connect a USB camera, the system finds its default driver and connects it with the camera. To override the system’s default matching behavior so that you can load a custom CMIO extension instead, create a simple DriverKit extension.

### Create a DriverKit extension

In a standalone Xcode project, or as a target within an existing project, create a new DriverKit extension. In Xcode’s menu, select File \> New and choose either the Project or Target menu items as appropriate. In the dialog that appears, select the DriverKit tab and the Driver template, and click the Next button.

In the dialog that follows, give the driver an appropriate Product Name and click the Finish button to create it.

The default IOKit interface generator (`.iig`) and C++ implementation files that the template creates provide the sufficient implementation for your driver. The driver is effectively codeless, but the system requires a minimal binary for entitlement purposes.

### Configure the Info.plist file

Specify your matching parameters as one or more entries in the IOKitPersonalities dictionary inside the DriverKit extension’s `Info.plist` file. The following example shows the standard configuration to provide within this file.

```
IOKitPersonalities

    Camera-Identifier

        CFBundleIdentifierKernel
        com.apple.UVCService
        IOClass
        UVCService
        IOProviderClass
        IOUSBHostInterface
        bConfigurationValue
        *
        bInterfaceNumber
        *
        14
        bInterfaceSubClass
        *
        IOUserClass
        [DRIVERKIT CLASS NAME]
        IOUserServerName
        [DRIVERKIT SERVER NAME]
        IOProbeScore
        9999
        idVendor
        123
        idProduct
        123
        IOProviderMergeProperties

            CameraAssistantBundleID
            [YOUR CMIO EXTENSION ID]

```

Set IOUserClass and IOUserServerName values as appropriate for your newly created extension. Set a high `IOProbeScore` value to give priority to your driver, and set the identifiers of the vendor and product to match. In the `IOProviderMergeProperties`, specify the identifier of your custom CMIO extension to load in place of the default driver.

With the configuration of your DriverKit extension complete, refer to Installing System Extensions and Drivers for information on how to package and install your extension.

## See Also

### Providers

Creating a camera extension with Core Media I/O

Build high-performance camera drivers that are secure and simple to deploy.

class CMIOExtensionProvider

An object that manages device connections for a provider.

protocol CMIOExtensionProviderSource

A protocol for objects that act as provider sources.

class CMIOExtensionProviderProperties

An object that manages the properties of an extension provider.

