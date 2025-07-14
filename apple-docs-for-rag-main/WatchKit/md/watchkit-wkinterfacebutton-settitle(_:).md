

- WatchKit
- WKInterfaceButton
-  setTitle(\_:) 

Instance Method

# setTitle(\_:)

Sets the button title to the specified string.

watchOS 2.0+

``` source
func setTitle(_ title: String?)
```

## Parameters 

`title`  

The text to display in the button. Specifying `nil` clears the current text from the button.

## Discussion

This method looks for a localized version of `title` in your WatchKit extension’s `Localizable.strings` file. If it finds one, it uses the localized string for the button title. If it does not find a localized version of the string, it uses the value in the `title` parameter directly. The text replaces the previous text set for the button.

The button text is drawn using the font and styling information from your storyboard. The text is drawn on top of the button’s background image or color.

## See Also

### Related Documentation

App Programming Guide for watchOS

### Setting the Button Title

func setAttributedTitle(NSAttributedString?)

Sets the button title to the specified attributed string.

