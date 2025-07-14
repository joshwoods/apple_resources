

- External Accessory
-  EAAccessoryKey 

Global Variable

# EAAccessoryKey

A key that indicates the accessory object whose status changed.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
let EAAccessoryKey: String
```

## Discussion

The EAAccessoryDidConnectNotification and EAAccessoryDidDisconnectNotification notifications contain this key in their userInfo dictionary. The value is an EAAccessory object.

## See Also

### Managing Connection Status Changes

func registerForLocalNotifications()

Begins the delivery of accessory-related notifications to the current application.

func unregisterForLocalNotifications()

Stops the delivery of accessory-related notifications to the current application.

static let EAAccessoryDidConnect: NSNotification.Name

A notification that the system sends when an accessory becomes connected and available for your application to use.

static let EAAccessoryDidDisconnect: NSNotification.Name

A notification that is posted when an accessory is disconnected and no longer available for your application to use.

let EAAccessorySelectedKey: String

A key that indicates the accessory object that the user selected.

