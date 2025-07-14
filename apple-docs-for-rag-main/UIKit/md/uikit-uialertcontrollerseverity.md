

- UIKit
-  UIAlertControllerSeverity 

Enumeration

# UIAlertControllerSeverity

Constants for specifying the severity of an alert in apps built with Mac Catalyst.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
enum UIAlertControllerSeverity
```

## Overview

This enumeration defines the severity options used by the severity property of UIAlertController. In apps built with Mac Catalyst, the severity determines the style of the presented alert. A UIAlertControllerSeverity.critical alert appears with a caution icon, and an alert with a UIAlertControllerSeverity.default severity doesn’t. UIKit ignores the alert severity on iOS.

You should only use the UIAlertControllerSeverity.critical severity if an alert truly requires special attention from the user. For more information, see the Human Interface Guidelines on alerts.

## Topics

### Constants

case critical

Indicates that the system should present the alert using the critical, or caution, style.

case `default`

Indicates that the system should present the alert using the standard alert style.

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

### Configuring alert severity

var severity: UIAlertControllerSeverity

Indicates the severity of the alert.

