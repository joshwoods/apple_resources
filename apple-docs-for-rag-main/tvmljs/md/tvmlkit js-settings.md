

- TVMLKit JS
-  Settings 

Class

# Settings

An object that provides access to setting information for a device.

tvOS 9.0+

``` source
interface Settings
```

## Overview

You cannot create an instance of the `Settings` class. An instance of this class is available in the global context as `Settings`.

## Topics

### Retrieving Setting Information

restrictions

Restriction information on the device.

language

The language used to display information by the device.

onRestrictionsChange

A callback function that is called when changes to a device’s restriction information changes.

storefrontCountryCode

The country code used by the store on this device.

## See Also

### Device Settings

Device

An object that provides information about an Apple TV and the host app installed on the device.

Restrictions

An object used to retrieve rating restriction information.

