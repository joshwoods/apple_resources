

- DeviceDiscoveryUI
-  DDDevicePickerViewController 

Class

# DDDevicePickerViewController

A UIKit view that displays other devices on the network, and creates an encrypted connection to a copy of your app running on that device.

tvOS 16.0+

``` source
@MainActor
class DDDevicePickerViewController
```

## Mentioned in 

Connecting a tvOS app to other devices over the local network

## Overview

Always display the device picker as a full-screen, modal view. If the user selects a device, the system sets the `endpoint` property and calls the `endpointPickedHandler`.

```
// This example uses the default application services parameters;
// however, you can add a NWProtocolFramer to provide application-level
// messaging.
let parameters = NWParameters.applicationService

// Create the view controller for the endpoint picker.
let devicePickerController =
DDDevicePickerViewController(browseDescriptor: NWBrowser.Descriptor.applicationService(name: "MyAppService"),
                               parameters: parameters)

// Show the network device picker as a full-screen, modal view.
devicePickerController.modalTransitionStyle = .coverVertical
show(devicePickerController, sender: nil)

let endpoint: NWEndpoint
do {
    endpoint = try await devicePickerController.endpoint
} catch {
    // The user canceled the endpoint picker view.
    return
}

// Use the endpoint here.
myDeviceConnectionManager.connectTo(endpoint: endpoint)
```

## Topics

### Creating device picker view controllers

static func isSupported(NWBrowser.Descriptor, using: NWParameters?) -> Bool

Returns a Boolean value that indicates whether the current device supports device discovery.

convenience init?(browseDescriptor: NWBrowser.Descriptor, parameters: NWParameters?)

Creates a view controller that displays the other, available devices on your local network.

### Accessing the selected endpoint

var endpoint: NWEndpoint

A network connection endpoint for the device selected by the user.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- Sendable
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Selecting nearby devices

Connecting a tvOS app to other devices over the local network

Display a view in your tvOS app that lists available iOS, iPadOS, and watchOS devices that the user can connect to over their local network.

struct DevicePicker

A SwiftUI view that displays other devices on the network, and creates an encrypted connection to a copy of your app running on that device.

struct DevicePickerSupportedAction

An environment value that indicates whether the current device supports device discovery.

NSApplicationServices

A list of service providers and the devices that they support.

