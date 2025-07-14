

- DeviceDiscoveryUI
-  DevicePickerSupportedAction 

Structure

# DevicePickerSupportedAction

An environment value that indicates whether the current device supports device discovery.

DeviceDiscoveryUISwiftUItvOS 16.0+

``` source
struct DevicePickerSupportedAction
```

## Overview

Access the action using the `.devicePickerSupports` key. Then call it as a function, passing the same browse descriptor and parameters you use to search for devices.

```
struct SettingsView: View {

    @Environment{\.devicePickerSupports} var myDevicePickerSupports
    @Binding var showDevicePicker: Bool

    var body: some View {
        if myDevicePickerSupports(.applicationService("MyAppService"),
                                  parameters: { .applicationService }) {
            Button("Select A Device") {
                // Display a device picker.
                showDevicePicker = true
            }
        }
    }
}
```

## Topics

### Checking for support

func callAsFunction(NWBrowser.Descriptor, parameters: (() -> NWParameters)?) -> Bool

Returns a Boolean value that indicates whether the current device supports device discovery.

## See Also

### Selecting nearby devices

Connecting a tvOS app to other devices over the local network

Display a view in your tvOS app that lists available iOS, iPadOS, and watchOS devices that the user can connect to over their local network.

struct DevicePicker

A SwiftUI view that displays other devices on the network, and creates an encrypted connection to a copy of your app running on that device.

class DDDevicePickerViewController

A UIKit view that displays other devices on the network, and creates an encrypted connection to a copy of your app running on that device.

NSApplicationServices

A list of service providers and the devices that they support.

