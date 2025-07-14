

- Core HID
-  Communicating with human interface devices 

Article

# Communicating with human interface devices

Interact with and obtain data from devices such as keyboards and mice.

## Overview

To communicate with a human interface device (HID), you must identify and match it using a set of matching critiera. When you match the device, you become its client and can query its properties and capabilities.

Note

Interacting with certain HIDs, such as keyboards, require user approval. Ensure that you grant permission to access the device to use it.

### Locate the device of interest

To locate the device you’re interested in, specify a set of matching criteria using HIDDeviceManager.DeviceMatchingCriteria. The following code uses this method to discover the Magic Keyboard with Numeric Keypad `product`:

```
```

Create a HIDDeviceManager and provide the criteria to monitorNotifications(matchingCriteria:). Notifications arrive immediately for connected devices, and later when newly connected matching devices appear. `monitorNotifications` returns an asynchronous stream that you iterate over. The loop awaits and releases the current Task until a notification comes in.

```
```

To specify matching criteria using additional properties, see init(primaryUsage:deviceUsages:vendorID:productID:transport:product:manufacturer:modelNumber:versionNumber:serialNumber:uniqueID:locationID:localizationCode:isBuiltIn:extraProperties:).

### Communicate with the device

Create a HIDDeviceClient and pass in the device reference to start communication with the device. Verify that you’re communicating with the correct device by checking the usage with primaryUsage, the transport with transport, and the product name with product.

```
```

Obtain the device’s input report using dispatchGetReportRequest(type:id:timeout:). Specify HIDReportType.input for the type, and provide the appropriate HIDReportID. This method initiates a get report request to the device over Bluetooth and returns the device’s response.

```
```

Monitor the device for input reports or other notifications by calling monitorNotifications(reportIDsToMonitor:elementsToMonitor:):

```
```

Raw reports provide detailed information about data going to and from the device; however, this can generate more detail than you need. Instead, use HIDElement to obtain specific information from a device.

For the keyboard in this example, the input report contains the report ID, status of the modifier keys, the currently pressed keys, vendor defined data and padding. To obtain just the state of the Shift key, obtain the corresponding element.

```
```

With `leftShiftKey`, monitor HIDDeviceClient.Notification.elementUpdates(values:) for any changes using HIDElement.Value. Values also arrive as a byte stream in bytes, but are interpretable as integers using extensions such as integerValue(asTypeTruncatingIfNeeded:). Because the Shift key state is 1 bit, treat it as a `UInt8`.

```
```

Use HIDElement with get and set reports through updateElements(_:timeout:). This takes HIDElement from HIDDeviceClient.RequestElementUpdate and HIDDeviceClient.ProvideElementUpdate, then issues get and set reports with the raw report data in the background.

The following example creates a unit test for the keyboard. It turns off the Caps Lock LED, queries the state of the left Shift key, turns on the Caps Lock LED, then queries the state of the left Shift key again to determine if toggling the LED alters the state of the left Shift key.

```
```

## See Also

### Interaction

actor HIDDeviceClient

A client of a physical or virtual HID compatible peripheral.

struct HIDElement

A representation of an item from a report descriptor for a HID device.

struct HIDElementCollection

A collection of items from a report descriptor for a HID device.

struct Value

Data associated with a HID element.

protocol HIDElementUpdate

A base protocol for element update types.

enum HIDReportType

Types for HID reports.

struct HIDReportID

A type to represent the report IDs of HID reports.

enum HIDUsage

A type to represent HID usage pages.

enum HIDDeviceError

Errors that the framework can throw.

enum HIDDeviceTransport

Common transport types that transmit data to or from a HID device.

enum HIDDeviceLocalizationCode

The localization codes that some HID devices declare to specify conformance to a certain format or language.

