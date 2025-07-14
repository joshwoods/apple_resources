

- WatchKit
- WKInterfaceTextField
-  setTextColor(\_:) 

Instance Method

# setTextColor(\_:)

Sets the text’s color.

watchOS 6.0+

``` source
func setTextColor(_ color: UIColor?)
```

## Parameters 

`color`  

The color to be applied to the text field’s text. Specifying `nil` removes the color and returns the text to the color specified in the storyboard file. The default color is white.

## Discussion

This method defines the default color of the entire string. The text field uses this color unless you explicitly override it in an attributed string using the NSForegroundColorAttributeName attribute.

## See Also

### Setting the Text

func setText(String?)

Sets the text displayed by the text field.

func setAttributedText(NSAttributedString?)

Sets the styled text displayed by the text field.

