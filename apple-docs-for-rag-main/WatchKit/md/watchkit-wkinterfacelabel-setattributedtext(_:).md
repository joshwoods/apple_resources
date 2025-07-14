

- WatchKit
- WKInterfaceLabel
-  setAttributedText(\_:) 

Instance Method

# setAttributedText(\_:)

Sets the label text to the specified attributed string.

watchOS 2.0+

``` source
func setAttributedText(_ attributedText: NSAttributedString?)
```

## Parameters 

`attributedText`  

The formatted text string to be displayed in the label. Specifying `nil` clears the current text from the label.

## Mentioned in 

Connecting Your User Interface to Your Code

## Discussion

This method changes the label text to the new value, replacing the old text if any. Any font and style attributes applied to the string take precedence over default values. If you do not explicitly specify font or styling information, the default values are used instead. For example, if you do not specify a text color explicitly, the default text color is used.

Attributed strings may not contain any NSTextAttachment objects as part of their content.

## See Also

### Setting the Label Text

func setText(String?)

Sets the label text to the specified string.

func setTextColor(UIColor?)

Sets the color to apply to plain text strings.

