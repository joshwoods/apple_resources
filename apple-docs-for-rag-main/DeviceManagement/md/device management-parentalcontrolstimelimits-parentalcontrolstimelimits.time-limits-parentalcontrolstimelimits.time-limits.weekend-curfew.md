

- Device Management
- ParentalControlsTimeLimits
- ParentalControlsTimeLimits.Time-limits
-  ParentalControlsTimeLimits.Time-limits.Weekend-curfew 

Device Management Profile

# ParentalControlsTimeLimits.Time-limits.Weekend-curfew

The weekend curfew dictionary.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ParentalControlsTimeLimits.Time-limits.Weekend-curfew
```

## Properties

`enabled`

`boolean`

 (Required) 

If `true`, enable these settings.

`end`

`string`

The curfew end time, in the format `%d:%d:%d`.

`rangeType`

`integer`

 (Required) 

The type of day range, which has the following possible values:

`0`  
Weekday

Possible Values: `0, 1`

`secondsPerDay`

`integer`

`start`

`string`

## Overview

`1`  
Weekend

- secondsPerDay: The allowance for that day, in seconds.

- start: The curfew start time, in the format `%d:%d:%d`.

## See Also

### Profiles

object ParentalControlsTimeLimits.Time-limits.Weekday-allowance

The weekday allowance dictionary.

object ParentalControlsTimeLimits.Time-limits.Weekday-curfew

The weekday curfew dictionary.

object ParentalControlsTimeLimits.Time-limits.Weekend-allowance

The weekend allowance dictionary.

