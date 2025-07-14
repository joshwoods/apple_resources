

- TVMLKit JS
- TVMLKit JS Functions
-  formatDuration 

Function

# formatDuration

Formats the given duration into the standard tvOS format.

tvOS 9.0+

``` source
String formatDuration(
    in int duration
);
```

## Parameters 

`duration`  

An integer specifying the duration, in seconds.

## Return Value

A string containing the formatted duration.

## Discussion

This function changes a number of seconds into the standard hour:minute:second format. For example, `formatDuration(90)` returns “1:30”.

## See Also

### Formatting Information

formatDate

Formats the given date into the given format.

formatNumber

Formats the specified number into the given format.

