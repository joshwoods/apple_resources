

- Foundation
- NSDateComponents
-  value(forComponent:) 

Instance Method

# value(forComponent:)

Returns the value for a given calendar unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(forComponent unit: NSCalendar.Unit) -> Int
```

## Parameters 

`unit`  

The calendar unit for which to retrieve its value. Do not pass calendar or timeZone.

## Return Value

The value for the given calendar unit.

## Discussion

This method allows for component values to be retrieved for an NSCalendar.Unit value.

## See Also

### Accessing Components as Calendrical Units

func setValue(Int, forComponent: NSCalendar.Unit)

Sets a value for a given calendar unit.

struct Unit

Calendrical units such as year, month, day and hour.

