

- WatchKit
- WKInterfaceLabel
-  setTextColor(\_:) 

Instance Method

# setTextColor(\_:)

Sets the color to apply to plain text strings.

watchOS 2.0+

``` source
func setTextColor(_ color: UIColor?)
```

## Parameters 

`color`  

The custom color to be applied to the label’s text. Specifying `nil` removes the custom color and returns the text to the color specified in the storyboard file. The default label color is white.

## Mentioned in 

Connecting Your User Interface to Your Code

## Discussion

The value set by this method represents the default color applied to text. This color is used unless you explicitly override it in an attributed string using the NSForegroundColorAttributeName attribute.

## See Also

### Setting the Label Text

func setText(String?)

Sets the label text to the specified string.

func setAttributedText(NSAttributedString?)

Sets the label text to the specified attributed string.

