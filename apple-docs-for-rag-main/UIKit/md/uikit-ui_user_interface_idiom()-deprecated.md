

- UIKit
-  UI_USER_INTERFACE_IDIOM() Deprecated

Function

# UI_USER_INTERFACE_IDIOM()

Returns the interface idiom supported by the current device (recommended for apps that run in versions of iOS earlier than 3.2).

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–11.0Deprecated

``` source
func UI_USER_INTERFACE_IDIOM() -> UIUserInterfaceIdiom
```

Deprecated

If your app runs in iOS 3.2 and later, use userInterfaceIdiom instead.

## Return Value

UIUserInterfaceIdiom.phone if the device is an iPhone or iPod touch or UIUserInterfaceIdiom.pad if the device is an iPad.

## See Also

### Getting the current idiom

enum UIUserInterfaceIdiom

Constants that indicate the interface type for the device or an object that has a trait environment, such as a view and view controller.

