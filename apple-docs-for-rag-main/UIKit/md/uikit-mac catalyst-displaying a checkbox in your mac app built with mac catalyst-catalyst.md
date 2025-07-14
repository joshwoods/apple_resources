

- UIKit
- Mac Catalyst
-  Displaying a checkbox in your Mac app built with Mac Catalyst 

Article

# Displaying a checkbox in your Mac app built with Mac Catalyst

Present a switch control as a Mac-style checkbox when your app runs in the Mac user interface idiom.

## Overview

A Mac app built with Mac Catalyst that uses the Mac user interface idiom displays a UISwitch as a checkbox when the preferredStyle value is UISwitch.Style.automatic (the default value) or UISwitch.Style.checkbox. If your app doesn’t use the UIUserInterfaceIdiom.mac idiom, the switch appears as a slider switch. To learn more, see Choosing a user interface idiom for your Mac app.

### Add text to the checkbox

To display text alongside the checkbox, set the title property.

```
let showFavoritesAtTop = UISwitch()
showFavoritesAtTop.title = "Always show favorite recipes at the top"
```

### Resize the checkbox

A checkbox-style switch has a default frame size of zero. If you’re not using Auto Layout to determine the size and position of the switch, call sizeToFit() to resize it so that it uses the appropriate amount of space needed to display the checkbox and its title.

## See Also

### User interface

UIKit Catalog: Creating and customizing views and controls

Customize your app’s user interface with views and controls.

Building and improving your app with Mac Catalyst

Improve your iPadOS app with Mac Catalyst by supporting native controls, multiple windows, sharing, printing, menus and keyboard shortcuts.

Removing the title bar in your Mac app built with Mac Catalyst

Display content that fills the entire height of a window by removing the title bar.

Toolbar

Provide a space for controls under a window’s title bar and above your custom content.

Touch Bar

Display interactive content and controls in the Touch Bar.

