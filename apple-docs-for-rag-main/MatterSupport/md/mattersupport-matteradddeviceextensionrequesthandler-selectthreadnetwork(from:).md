

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  selectThreadNetwork(from:) 

Instance Method

# selectThreadNetwork(from:)

Provides the visible Thread networks to the device.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
func selectThreadNetwork(from threadScanResults: [MatterAddDeviceExtensionRequestHandler.ThreadScanResult]) async throws -> MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation
```

## Return Value

The Thread network to join, or defaultSystemNetwork.

## Discussion

The Matter device provides information about the visible Thread networks that it sees. This allows the ecosystem to choose the correct network for the device to use.

The system may provide the selected Thread network in the completion handler. The device commissions onto the specified network. The device must be able to send the device IP traffic after it associates to the given network. Otherwise, if the system returns defaultSystemNetwork, the device commissions onto the Preferred Thread network known to the device.

Store credentials for the provided Thread network by calling storeCredentials(forBorderAgent:activeOperationalDataSet:completion:) before completing this callback.

If the Matter device is already commissioned with a network, the selected network may do nothing.

## See Also

### Selecting the Thread network

struct ThreadScanResult

A result of a Thread-scan operation performed on the device

struct ThreadNetworkAssociation

The description of an association to a Thread network.

