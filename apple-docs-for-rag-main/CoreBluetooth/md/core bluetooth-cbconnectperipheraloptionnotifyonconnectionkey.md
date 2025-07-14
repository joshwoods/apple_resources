

- Core Bluetooth
-  CBConnectPeripheralOptionNotifyOnConnectionKey 

Global Variable

# CBConnectPeripheralOptionNotifyOnConnectionKey

A Boolean value that specifies whether the system should display an alert when connecting a peripheral in the background.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.13+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBConnectPeripheralOptionNotifyOnConnectionKey: String
```

## Discussion

The value for this key is an NSNumber object. This key is useful for apps that haven’t specified the `bluetooth-central` background mode and can’t display their own alert. If more than one app requests a notification for a given peripheral, the one that was most recently in the foreground receives the alert. If the key isn’t specified, the default value is false.

## See Also

### Options

let CBConnectPeripheralOptionEnableAutoReconnect: String

A Boolean value that specifies whether the system automatically reconnects with a peripheral.

let CBConnectPeripheralOptionEnableTransportBridgingKey: String

An option to bridge classic Bluetooth technology profiles, if already connected over Bluetooth Low Energy.

let CBConnectPeripheralOptionNotifyOnDisconnectionKey: String

A Boolean value that specifies whether the system should display an alert when disconnecting a peripheral in the background.

let CBConnectPeripheralOptionNotifyOnNotificationKey: String

A Boolean value that specifies whether the system should display an alert for any notification sent by a peripheral.

let CBConnectPeripheralOptionRequiresANCS: String

An option to require Apple Notification Center Service (ANCS) when connecting a device.

let CBConnectPeripheralOptionStartDelayKey: String

An option that indicates a delay before the system makes a connection.

