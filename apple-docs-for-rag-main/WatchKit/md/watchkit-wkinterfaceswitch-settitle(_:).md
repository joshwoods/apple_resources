

- WatchKit
- WKInterfaceSwitch
-  setTitle(\_:) 

Instance Method

# setTitle(\_:)

Sets the switch title to the specified string.

watchOS 2.0+

``` source
func setTitle(_ title: String?)
```

## Parameters 

`title`  

The text to be displayed in the switch. Specifying `nil` clears the current text from the switch.

## Discussion

This method looks for a localized version of title in your WatchKit extension’s `Localizable.strings` file. If it finds one, it uses the localized string for the switch title. If it does not find a localized version of the string, it uses the value in the title directly. The text replaces the previous text set for the switch.

The switch title is drawn using the font and styling information from your storyboard.

## See Also

### Related Documentation

App Programming Guide for watchOS

### Setting the Switch’s Title

func setAttributedTitle(NSAttributedString?)

Sets the switch title to the specified attributed string.

