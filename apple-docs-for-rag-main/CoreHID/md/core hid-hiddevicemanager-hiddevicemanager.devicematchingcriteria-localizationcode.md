

- Core HID
- HIDDeviceManager
- HIDDeviceManager.DeviceMatchingCriteria
-  localizationCode 

Instance Property

# localizationCode

A localization code that specifies the HID compliant localization code.

macOS 15.0+

``` source
var localizationCode: HIDDeviceLocalizationCode?
```

## Discussion

The localization code can specify for which specific format the device is localized. For example, a Japanese (JIS) keyboard declares the HIDDeviceLocalizationCode.japan localization code.

