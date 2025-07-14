

- WatchKit
- WKInterfaceLabel
-  setText(\_:) 

Instance Method

# setText(\_:)

Sets the label text to the specified string.

watchOS 2.0+

``` source
func setText(_ text: String?)
```

## Parameters 

`text`  

The text to be displayed in the label. Specifying `nil` clears the current text from the label.

## Mentioned in 

Connecting Your User Interface to Your Code

## Discussion

This method changes the string displayed by the label to the new value. When using this method to set the text, the default font and styling information for the text is derived from the storyboard file. You can change the default text color using the setTextColor(_:) method.

Changing the text of the label causes the label to resize itself to accommodate the new string. If the string is too large to fit the available space, WatchKit truncates the text.

## See Also

### Related Documentation

App Programming Guide for watchOS

### Setting the Label Text

func setTextColor(UIColor?)

Sets the color to apply to plain text strings.

func setAttributedText(NSAttributedString?)

Sets the label text to the specified attributed string.

