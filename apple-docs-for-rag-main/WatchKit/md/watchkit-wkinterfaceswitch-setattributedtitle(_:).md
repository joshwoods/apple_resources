

- WatchKit
- WKInterfaceSwitch
-  setAttributedTitle(\_:) 

Instance Method

# setAttributedTitle(\_:)

Sets the switch title to the specified attributed string.

watchOS 2.0+

``` source
func setAttributedTitle(_ attributedTitle: NSAttributedString?)
```

## Parameters 

`attributedTitle`  

The formatted text string to be displayed in the switch. Specifying `nil` clears the current text from the switch.

## Discussion

This method sets the content of the switch to the specified text, replacing the previous text. The text is drawn using the style information in `attributedTitle`.

If you use styled text in your switches, you must provide localized versions of the text yourself. Attributed strings may not contain any NSTextAttachment objects as part of their content.

## See Also

### Setting the Switch’s Title

func setTitle(String?)

Sets the switch title to the specified string.

