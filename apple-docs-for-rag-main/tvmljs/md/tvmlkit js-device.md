

- TVMLKit JS
-  Device 

Class

# Device

An object that provides information about an Apple TV and the host app installed on the device.

tvOS 9.0+

``` source
interface Device
```

## Overview

You cannot create an instance of the `Device` class. An instance of this class is available in the global context as `Device`.

## Topics

### Retrieving Device Information

appIdentifier

The unique identifier for the app.

appVersion

The current app version.

model

A string that identifies the device model.

productType

The version of the product installed on the Apple TV.

systemVersion

The tvOS version.

vendorIdentifier

The universally unique identifier (UUID) of the device.

## See Also

### Device Settings

Settings

An object that provides access to setting information for a device.

Restrictions

An object used to retrieve rating restriction information.

