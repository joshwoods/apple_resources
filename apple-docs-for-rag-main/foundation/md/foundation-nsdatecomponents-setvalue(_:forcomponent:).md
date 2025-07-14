

- Foundation
- NSDateComponents
-  setValue(\_:forComponent:) 

Instance Method

# setValue(\_:forComponent:)

Sets a value for a given calendar unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setValue(
    _ value: Int,
    forComponent unit: NSCalendar.Unit
)
```

## Parameters 

`value`  

The value to set for the `unit` component.

`unit`  

The calendar unit for which to set `value`. Do not pass calendar or timeZone.

## Discussion

This method allows for component values to be set for an NSCalendar.Unit value.

## See Also

### Accessing Components as Calendrical Units

func value(forComponent: NSCalendar.Unit) -> Int

Returns the value for a given calendar unit.

struct Unit

Calendrical units such as year, month, day and hour.

