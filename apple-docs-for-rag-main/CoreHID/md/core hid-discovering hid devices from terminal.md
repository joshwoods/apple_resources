

- Core HID
-  Discovering HID devices from Terminal 

Article

# Discovering HID devices from Terminal

Identify devices connected to your Mac from the command line.

## Overview

To interact with a human interface device (HID), you must identify what devices are available on your system. The `hidutil` command is a human interface device utility that you can use to probe a Mac for HID devices, monitor HID events, and to obtain device reports. Run `hidutil list` in Terminal (`/Applications/Utilities`) to receive a list of HID devices. The `Devices` portion of the output is relevant for discovering available human interface devices.

```
```

There are multiple entries with similar product names. Some products register as multiple devices to segment functionality that you match and interact with individually. For example, a device may have a keyboard and trackpad in the same form factor, but declare them as two separate components.

The `UsagePage` column contains the usage page, which is a category of broad functionality. In the above output, the usage page is either `1` or `65280`. According to HID Usage Tables for Universal Serial Bus (USB), `65280 (0xFF00)` is a vendor-defined page and is reserved for the vendor to use as they see fit; therefore, ignore any entries with this page. Usage page `1` is the Generic Desktop page. Because both a keyboard and a mouse are Generic Desktop devices, you must further refine the search by examining the usage value.

Values in the `Usage` column relate to a category of specific functionality. In the output above, items with a usage page of `1` have a usage value of `2` or `6`, defined as a mouse or keyboard, respectively, according to HID Usage Tables for Universal Serial Bus (USB).

## See Also

### Discovery

actor HIDDeviceManager

A helper for discovering human interface devices (HID) connected to the system.

struct DeviceMatchingCriteria

Matching criteria used to filter HID devices.

