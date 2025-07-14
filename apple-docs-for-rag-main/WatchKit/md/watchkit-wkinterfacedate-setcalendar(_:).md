

- WatchKit
- WKInterfaceDate
-  setCalendar(\_:) 

Instance Method

# setCalendar(\_:)

Sets the calendar to use when formatting date information.

watchOS 2.0+

``` source
func setCalendar(_ calendar: Calendar?)
```

## Parameters 

`calendar`  

The calendar to be used. Specifying nil removes the calendar information and causes Apple Watch to use the default calendar based on the user’s settings.

## Discussion

Use this method to configure the calendar to one that is different from the user’s current calendar. You might change the calendar to format dates differently based on your app’s needs. For example, a financial reporting app might use a calendar that breaks the year into fiscal quarters rather than months.

## See Also

### Configuring the Date and Time Display

func setTextColor(UIColor?)

Sets the color of the date and time text.

func setTimeZone(TimeZone?)

Sets the time zone to use when displaying time information.

