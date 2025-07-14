

- UIKit
- UISwitch
-  preferredStyle 

Instance Property

# preferredStyle

The preferred display style for the switch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var preferredStyle: UISwitch.Style { get set }
```

## Mentioned in 

Displaying a checkbox in your Mac app built with Mac Catalyst

Choosing a user interface idiom for your Mac app

## Discussion

Use this property to specify the display style that you prefer. If the style changes, the switch may generate a layout pass to update the display.

The default style is UISwitch.Style.automatic. For a list of styles, see UISwitch.Style.

## See Also

### Setting the display style

Displaying a checkbox in your Mac app built with Mac Catalyst

Present a switch control as a Mac-style checkbox when your app runs in the Mac user interface idiom.

var style: UISwitch.Style

The display style for the switch.

enum Style

Styles that determine the appearance of the switch.

var title: String?

The title displayed next to a checkbox-style switch.

