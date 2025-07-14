

- WatchKit
- WKInterfaceButton
-  setAttributedTitle(\_:) 

Instance Method

# setAttributedTitle(\_:)

Sets the button title to the specified attributed string.

watchOS 2.0+

``` source
func setAttributedTitle(_ attributedTitle: NSAttributedString?)
```

## Parameters 

`attributedTitle`  

The formatted text string to be displayed in the button. Specifying `nil` clears the current text from the button.

## Discussion

This method sets the content of the button to the specified text, replacing the previous text. The text is drawn using the style information in `attributedTitle`. If the button has a background image, the text is drawn on top of that image.

If you use styled text in your buttons, you must provide localized versions of the text yourself. Attributed strings may not contain any NSTextAttachment objects as part of their content.

## See Also

### Setting the Button Title

func setTitle(String?)

Sets the button title to the specified string.

