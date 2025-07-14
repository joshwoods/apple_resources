

- Core Bluetooth
-  CBConnectPeripheralOptionStartDelayKey 

Global Variable

# CBConnectPeripheralOptionStartDelayKey

An option that indicates a delay before the system makes a connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.13+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBConnectPeripheralOptionStartDelayKey: String
```

## Discussion

The corresponding value is an NSNumber that indicates the duration of the delay in seconds.

## See Also

### Options

let CBConnectPeripheralOptionEnableAutoReconnect: String

A Boolean value that specifies whether the system automatically reconnects with a peripheral.

let CBConnectPeripheralOptionEnableTransportBridgingKey: String

An option to bridge classic Bluetooth technology profiles, if already connected over Bluetooth Low Energy.

let CBConnectPeripheralOptionNotifyOnConnectionKey: String

A Boolean value that specifies whether the system should display an alert when connecting a peripheral in the background.

let CBConnectPeripheralOptionNotifyOnDisconnectionKey: String

A Boolean value that specifies whether the system should display an alert when disconnecting a peripheral in the background.

let CBConnectPeripheralOptionNotifyOnNotificationKey: String

A Boolean value that specifies whether the system should display an alert for any notification sent by a peripheral.

let CBConnectPeripheralOptionRequiresANCS: String

An option to require Apple Notification Center Service (ANCS) when connecting a device.

