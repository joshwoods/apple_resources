

- TVMLKit JS
- Settings
-  onRestrictionsChange 

Instance Property

# onRestrictionsChange

A callback function that is called when changes to a device’s restriction information changes.

tvOS 9.0+

``` source
attribute function onRestrictionsChange;
```

## Discussion

The `onRestrictionsChange` attribute is used to update any activities that use a device’s restriction information. The attribute must be set to a function; for example, `Settings.onRestrictionsChange = function () {}`.

## See Also

### Retrieving Setting Information

restrictions

Restriction information on the device.

language

The language used to display information by the device.

storefrontCountryCode

The country code used by the store on this device.

