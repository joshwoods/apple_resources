

- MatterSupport
-  Adding Matter support to your ecosystem 

Article

# Adding Matter support to your ecosystem

Allow people to add Matter accessories to your platform.

## Overview

With the MatterSupport framework, you can administer, add, and configure Matter devices in your ecosystem using an iOS device. To onboard a device, you need to configure discovery, set up a home, create an extension request handler, and override its methods.

### Configure discovery

Add the following to your app’s `Info.plist` so it can discover Matter-related services. See NSBonjourServices for more information.

```
NSBonjourServices

        _matter._tcp
        _matterc._udp
        _matterd._udp

```

### Set up the home

Define the home’s name, then create the topology and pass your ecosystem name and an array of homes.

```
```

Use the newly created topology object to create a request to add a device.

```
```

You can optionally provide the Matter setup code programmatically while setting up a Matter device in an ecosystem. To do this, pass a string containing the payload information from the device’s packaging, such as a QR code. For more information on when this is appropriate, see Matter Allow Setup Payload.

```
```

Next, start the user interface flow for adding the device. Handle any errors that may occur during the setup.

```
```

### Create the extension request handler

Subclass MatterAddDeviceExtensionRequestHandler and override its methods. This class facilitates the user interface flow during the setup of a new Matter device.

```
```

### Set the principal class

Register the subclass you created above in the app’s `Info.plist` as the NSPrincipalClass for the `com.apple.matter.support.extension.device-setup` extension point identifier.

## See Also

### Adding a device

struct MatterAddDeviceRequest

A request that adds and sets up a device into an ecosystem.

class MatterAddDeviceExtensionRequestHandler

The object that handles configuration and commissioning of a device into an ecosystem.

