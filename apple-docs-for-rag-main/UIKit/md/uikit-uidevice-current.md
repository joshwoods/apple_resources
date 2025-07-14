

- UIKit
- UIDevice
-  current 

Type Property

# current

An object that represents the current device.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class var current: UIDevice { get }
```

## Return Value

A singleton object that represents the current device.

## Discussion

You access the properties of the returned UIDevice instance to obtain information about the device. You must instantiate the UIDevice instance before registering to receive device notifications.

