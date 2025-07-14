

- Core HID
- HIDVirtualDevice
- HIDVirtualDevice.Properties
-  localizationCode 

Instance Property

# localizationCode

A device localization code that specifies the HID compliant localization code.

macOS 15.0+

``` source
let localizationCode: HIDDeviceLocalizationCode?
```

## Discussion

The localization code can specify the specific format a device is localized. For example, a Japanese (JIS) keyboard should declare the HIDDeviceLocalizationCode.japan localization code.

