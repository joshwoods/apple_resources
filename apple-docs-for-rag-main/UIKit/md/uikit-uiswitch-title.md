

- UIKit
- UISwitch
-  title 

Instance Property

# title

The title displayed next to a checkbox-style switch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var title: String? { get set }
```

## Mentioned in 

Choosing a user interface idiom for your Mac app

Displaying a checkbox in your Mac app built with Mac Catalyst

## Discussion

Set title only when the user interface idiom is UIUserInterfaceIdiom.mac; otherwise, a runtime exception occurs.

```
let showFavoritesAtTop = UISwitch()
showFavoritesAtTop.preferredStyle = .checkbox
if traitCollection.userInterfaceIdiom == .mac {
    showFavoritesAtTop.title = "Always show favorite recipes at the top"
}
```

The switch ignores title when the value of style isn’t UISwitch.Style.checkbox.

## See Also

### Setting the display style

Displaying a checkbox in your Mac app built with Mac Catalyst

Present a switch control as a Mac-style checkbox when your app runs in the Mac user interface idiom.

var preferredStyle: UISwitch.Style

The preferred display style for the switch.

var style: UISwitch.Style

The display style for the switch.

enum Style

Styles that determine the appearance of the switch.

