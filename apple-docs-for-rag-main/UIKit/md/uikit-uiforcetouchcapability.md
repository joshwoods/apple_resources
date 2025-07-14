

- UIKit
-  UIForceTouchCapability 

Enumeration

# UIForceTouchCapability

Keys that indicate the availability of 3D Touch on a device.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UIForceTouchCapability
```

## Overview

Only certain devices support 3D Touch. On those that do, the user can disable 3D Touch in the Accessibility area in Settings.

## Topics

### Availability options

case unknown

The availability of 3D Touch is unknown.

case available

3D Touch is available on the device.

case unavailable

3D Touch isn’t available on the device.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Retrieving the force touch capability traits

var forceTouchCapability: UIForceTouchCapability

The force touch capability value of the trait collection.

