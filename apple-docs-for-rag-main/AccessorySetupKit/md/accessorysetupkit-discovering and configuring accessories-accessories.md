

- AccessorySetupKit
-  Discovering and configuring accessories 

Article

# Discovering and configuring accessories

Detect nearby accessories and facilitate their setup.

## Overview

Use the AccessorySetupKit framework to simplify discovery and configuration of Bluetooth or Wi-Fi accessories. This allows the person using your app to use these devices without granting overly-broad Bluetooth or Wi-Fi access.

To discover accessories and present them in your app:

1.  Declare that your app uses AccessorySetupKit in its information property list.

2.  In your app, create and activate an instance of ASAccessorySession.

3.  Provide information about your supported accessories to display a picker. This lets the person using your app discover and select nearby accessories to configure.

4.  When the picker sends an accessory added event, use information about the selected device to create a Bluetooth or Wi-Fi connection.

### Declare your app’s accessories

To prepare your app to discover accessories, add the `NSAccessorySetupKitSupports` key to its information property list. Set its value to an array of strings that contains one or more of the following values:

`Bluetooth`  
Add this value if your app discovers accessories using Bluetooth or Bluetooth Low Energy.

`WiFi`  
Add this value if your app discovers accessories by finding Wi-Fi SSIDs that the accessories publish.

If you add `Bluetooth` to the list of supported protocols, you also need to add the following keys and values to your app’s information property list:

`NSAccessorySetupBluetoothCompanyIdentifiers`  
An array of strings that represent the Bluetooth company identifiers for accessories your app configures.

`NSAccessorySetupBluetoothNames`  
An array of strings that represent the Bluetooth device names for accessories your app configures.

`NSAccessorySetupBluetoothServices`  
An array of strings that represent the hexadecimal values of Bluetooth services for accessories your app configures.

Important

If your app tries to discover Bluetooth accessories during setup without supplying these keys and values, or uses identifiers, names, or services that it doesn’t include in its information property list, the app crashes. This only affects use of AccessorySetupKit discovery and selection; you can use other services and properties on the accessory after the person using the app selects it.

### Activate a discovery session

The ASAccessorySession is how your app uses the AccessorySetupKit framework. In your app, you create an instance of ASAccessorySession and activate it to receive callbacks with events as the session processes events. The activate(on:eventHandler:) method takes a DispatchQueue and an event-handling block or closure. The callbacks occur on the provided queue, which defaults to main.

The event handler receives a single parameter of type ASAccessoryEvent, which has an eventType that you use to determine what to do with each callback. For example, shortly after activating the session, your callback receives the ASAccessoryEventType.activated event. The following listing comments on the meaning of these events and how you may want to handle them.

```
```

### Display an accessory picker

When the session activates, its accessories array contains any accessories previously authorized for the app, which you can inspect. To discover new devices, your app needs to show an accessory picker. The person using the app uses this picker to choose the accessory to configure.

Note

If someone renames a previously-discovered Wi-Fi accessory, it becomes discoverable again by the picker.

Create instances of ASPickerDisplayItem that describe the items in the session that your app can configure. Collect these items in an array and pass them to the session for the operating system to present a picker:

```
```

Each display item’s descriptor, a property of type ASDiscoveryDescriptor, needs to have a bluetoothCompanyIdentifier or bluetoothServiceUUID, and at least one of the following accessory identifiers:

- bluetoothNameSubstring

- A bluetoothManufacturerDataBlob and bluetoothManufacturerDataMask set to the same length.

- A bluetoothServiceDataBlob and bluetoothServiceDataMask set to the same length.

- Either ssid or ssidPrefix, which needs to have a non-zero length. Only supply one of these; the app crashes if you supply both.

For Bluetooth accessories, the accessory identifiers you use in display items need to match the values you supply in the app’s information property list.

Along with filtering matched accessories to show in the picker, the display item and its descriptor allow you to control certain behaviors of the picker interaction. You can limit the bluetoothRange of the descriptor to only match accessories in the immediate physical proximity of the device running the app. To specify behaviors like allowing renaming of the accessory during setup, or confirming accessory authorization before showing the setup view, set the display item’s setupOptions.

When the picker appears, the person using the app sees a view of all nearby accessories that match the identifiers you provide. When multiple devices match a given identifier, the picker shows a separate item for each unique device. This allows the person to select a single device with the picker.

### Use the picker when migrating to AccessorySetupKit

You can also perform a one-time migration of previously-configured accessories, which adds them to the AccessorySetupKit framework’s list of known accessories. To do this, create instances of ASMigrationDisplayItem and include them in the array of items you send to showPicker(for:completionHandler:).

For items you want to migrate, set one or both of the following:

- A hotspotSSID, which must be a full SSID and not a prefix.

- A peripheralIdentifier, which corresponds to the identifier property of the CBPeer type.

Important

Don’t initialize a CBCentralManager before migration is complete. If you do, your callback handler receives an error and the picker fails to appear.

### Connect and configure the selected device

When the person picks an accessory, the picker sends an event of type ASAccessoryEventType.accessoryAdded, followed by an ASAccessoryEventType.pickerDidDismiss event when they dismiss the picker. If your app presents its own UI to configure the accessory, wait for the picker to dismiss, then use the accessory from the first event. You can handle this scenario by rewriting your event handler closure from before as follows, storing the accessory on the first event and retrieving it on the second.

```
```

The event’s accessory property contains details of the selected device, like its displayName and an bluetoothIdentifier for Bluetooth devices or ssid for Wi-Fi. Use this information to connect to the accessory — using Core Bluetooth for Bluetooth or Network Extension for Wi-Fi — and begin your device-specific setup process.

```
```

Because the app discovered the device with AccessorySetupKit, connecting to the device won’t invoke the TCC or other alerts that the system normally shows when using these system frameworks.

## See Also

### Essentials

Authorizing a Bluetooth accessory to share a dice roll

Discover, select, and set up a specific Bluetooth accessory without requesting permission to use Bluetooth.

class ASAccessorySession

A class to coordinate accessory discovery.

