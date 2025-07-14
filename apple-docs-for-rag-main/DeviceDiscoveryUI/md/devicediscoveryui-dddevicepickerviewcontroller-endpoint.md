

- DeviceDiscoveryUI
- DDDevicePickerViewController
-  endpoint 

Instance Property

# endpoint

A network connection endpoint for the device selected by the user.

tvOS 16.0+

``` source
@MainActor @preconcurrency
var endpoint: NWEndpoint { get async throws }
```

## Discussion

Your app can asynchronously read from this property. The system populates this property when the user selects a device from the endpoint picker. If the user cancels the picker, the system throws an error.

```
let endpoint: NWEndpoint
do {
    endpoint = try await myEndpointPickerHandler.endpoint
} catch {
    // The user canceled the endpoint picker view.
    return
}

// Use the endpoint here.
myDeviceConnectionManager.connectTo(endpoint: endpoint)
```

