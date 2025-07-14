

- DriverKit
-  Creating drivers for iPadOS 

Article

# Creating drivers for iPadOS

Bring your drivers to iPadOS by using the platform’s DriverKit support.

## Overview

In iPadOS 16 and later, you can develop drivers that run on macOS and iPadOS using DriverKit. The DriverKit frameworks provide a safe and secure approach to creating drivers for external USB and Thunderbolt devices that people can connect to their iPad.

iPadOS 16 supports the core DriverKit framework, as well as the following:

- USBDriverKit

- PCIDriverKit

- AudioDriverKit

Note

DriverKit on iPadOS requires an iPad with an M-series chip.

### Add a DriverKit target to your Xcode project

If you’re creating a new app in Xcode, use the Multiplatform App template when you create your project in Xcode. The app you create is what people use to install and update your driver on their macOS and iPadOS devices. To add a driver to your project, add a new target to your project by choosing DriverKit from the tab bar, and select the Driver target.

If you already have a DriverKit project for macOS, you can support iPadOS by editing your project settings. Select the project from the Navigator, select the app target, and choose General from the tab bar. In the Supported Destinations section, use the Add (+) button to add a new iPad destination.

### Install a driver

On macOS, your host app uses the System Extensions framework to install a driver onto the host system. On iPadOS, this framework is absent, so this step is unneccessary. If you’re writing a driver to run on both platforms, conditionalize your app code so you only call System Extensions on macOS.

```
```

Because drivers operate with enhanced privileges, a person using the device needs to approve any driver before it can run. On macOS, they grant this permission in System Settings \> Privacy & Security.

On iPadOS, there are two locations in the Settings app for managing drivers:

- If the iPad has at least one driver installed, Settings \> General \> Drivers lists all available drivers on the device. A person using the iPad can toggle each driver on or off individually.

- If your app contains a Settings bundle, Settings \> Your-App-Name \> Drivers lists the drivers installed by your app, with toggles to enable them. Your app needs to prompt the person to enable the driver in the Settings app.

After receiving permission, the driver runs on-demand. For example, a driver for an audio interface only runs when someone connects that hardware to their device.

### Allow user clients to attach to your driver

Some apps need to communicate with a running driver. The sample code project, Communicating between a DriverKit extension and a client app, provides an example of how to do this.

To allow user clients to connect to your driver, you need specific entitlements, based on the nature of your driver.

- On macOS, use the com.apple.developer.driverkit.userclient-access entitlement. Provide an array of allowed bundle identifiers as the value of this entitlement. Only apps with these bundle identifiers can connect to the driver at runtime.

- On iPadOS, use the Communicates with Drivers entitlement. This entitlement takes a Boolean value; set it to `YES` to allow your user client to connect to drivers.

- If your iPadOS driver works with many apps, use the DriverKit Allow Third Party User Clients entitlement. Set the Boolean value of this entitlement to `YES` to allow any app to connect to your driver.

## See Also

### Essentials

Implementing drivers, system extensions, and kexts

Create drivers and system extensions to communicate with hardware and provide low-level services, and only use kernel extensions for a few tasks.

