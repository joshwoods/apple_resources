

- WatchKit
- WKInterfaceTimer
-  setTextColor(\_:) 

Instance Method

# setTextColor(\_:)

Sets the color of the timer’s text.

watchOS 2.0+

``` source
func setTextColor(_ color: UIColor?)
```

## Parameters 

`color`  

The custom color to apply to the timer string. Specifying `nil` removes the custom color and returns the text to the color specified in the storyboard file. The default text color is white.

## See Also

### Configuring the Timer Attributes

func setDate(Date)

Changes the start time for the timer.

