

- WatchKit
- WKInterfaceDate
-  setTextColor(\_:) 

Instance Method

# setTextColor(\_:)

Sets the color of the date and time text.

watchOS 2.0+

``` source
func setTextColor(_ color: UIColor?)
```

## Parameters 

`color`  

The custom color to be applied to the time string. Specifying `nil` removes the custom color and returns the text to the color specified in the storyboard file. The default text color is white.

## See Also

### Related Documentation

App Programming Guide for watchOS

### Configuring the Date and Time Display

func setTimeZone(TimeZone?)

Sets the time zone to use when displaying time information.

func setCalendar(Calendar?)

Sets the calendar to use when formatting date information.

