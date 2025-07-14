

- UIKit
- UISwitch
-  UISwitch.Style 

Enumeration

# UISwitch.Style

Styles that determine the appearance of the switch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
enum Style
```

## Topics

### Styles

case automatic

A style indicating that the system chooses the appearance of the switch according to the current user interface idiom.

case checkbox

A style indicating that the switch appears as a Mac-style checkbox.

case sliding

A style indicating that the switch appears as an on/off slider.

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

### Setting the display style

Displaying a checkbox in your Mac app built with Mac Catalyst

Present a switch control as a Mac-style checkbox when your app runs in the Mac user interface idiom.

var preferredStyle: UISwitch.Style

The preferred display style for the switch.

var style: UISwitch.Style

The display style for the switch.

var title: String?

The title displayed next to a checkbox-style switch.

