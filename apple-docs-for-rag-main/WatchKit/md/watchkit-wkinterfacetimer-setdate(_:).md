

- WatchKit
- WKInterfaceTimer
-  setDate(\_:) 

Instance Method

# setDate(\_:)

Changes the start time for the timer.

watchOS 2.0+

``` source
func setDate(_ date: Date)
```

## Parameters 

`date`  

The new starting time for the timer. Specifying the current date or a date in the past causes the timer to count upward from that time. Specifying a date in the future causes the timer to count down to the specified time.

## Discussion

This method updates the target value but does not automatically update the timer display. You must call the timer’s start() method to begin updating the text it displays. When you do, the timer text is updated based on the time you set using this method.

## See Also

### Related Documentation

App Programming Guide for watchOS

func start()

Begins updates to the timer’s display.

### Configuring the Timer Attributes

func setTextColor(UIColor?)

Sets the color of the timer’s text.

