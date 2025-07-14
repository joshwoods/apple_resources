

- UIKit
- UISwitch
-  style 

Instance Property

# style

The display style for the switch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var style: UISwitch.Style { get }
```

## Discussion

This property returns the resolved style based on the user interface idiom, and never returns UISwitch.Style.automatic.

## See Also

### Setting the display style

Displaying a checkbox in your Mac app built with Mac Catalyst

Present a switch control as a Mac-style checkbox when your app runs in the Mac user interface idiom.

var preferredStyle: UISwitch.Style

The preferred display style for the switch.

enum Style

Styles that determine the appearance of the switch.

var title: String?

The title displayed next to a checkbox-style switch.

