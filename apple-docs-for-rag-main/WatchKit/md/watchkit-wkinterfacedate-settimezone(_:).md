

- WatchKit
- WKInterfaceDate
-  setTimeZone(\_:) 

Instance Method

# setTimeZone(\_:)

Sets the time zone to use when displaying time information.

watchOS 2.0+

``` source
func setTimeZone(_ timeZone: TimeZone?)
```

## Parameters 

`timeZone`  

The time zone to be used. Specifying `nil` removes the time zone information and causes Apple Watch to use the current time zone based on the user’s settings.

## Discussion

Use this method to configure the time zone to one that is different from the user’s current time zone. For example, a world clock app might use this method to configure the time display information.

## See Also

### Configuring the Date and Time Display

func setTextColor(UIColor?)

Sets the color of the date and time text.

func setCalendar(Calendar?)

Sets the calendar to use when formatting date information.

