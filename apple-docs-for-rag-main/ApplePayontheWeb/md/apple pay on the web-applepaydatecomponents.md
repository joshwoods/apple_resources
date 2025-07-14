

- Apple Pay on the Web
-  ApplePayDateComponents 

Structure

# ApplePayDateComponents

A dictionary that specifies the values for the calendrical units for a date.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayDateComponents {
 long years;
 long months;
 long days;
 long hours;
};
```

## Overview

When specifying a range using date components, provide all elements of the ApplePayDateComponents down to the level of granularity that you want to expose. For example, if you specify a range of days, be sure to include values for both months and years in addition to days in the ApplePayDateComponents.

Apple Pay on the Web uses the Gregorian calendar when processing dates.

## Topics

### Date Components

years

A number that represents a year.

months

A number between 1 and 12 that represents a month.

days

A number that represents a day.

hours

A number that represents an hour.

## See Also

### Start and End Dates of the Range

startDateComponents

The start date and time of the range.

endDateComponents

The end date and time of the range.

