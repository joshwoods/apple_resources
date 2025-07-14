

- SiriKit Cloud Media
-  DateComponents 

Type

# DateComponents

A full or partial date and time.

SiriKit Cloud Media 1.0.2+

``` source
* DateComponents
```

## Attributes 

Possible types: `string(/[0-9]{4}/)``, ``string(/[0-9]{4}-[0-9]{2}/)``, ``date``, ``date-time``, `ExplicitDateComponents

## Discussion

The client may provide an ExplicitDateComponents object or represent a Gregorian date in one of the following formats:

| Description | Format | Example |
|----|----|----|
| Year only | `string` (pattern: `/[0-9]{4}/)` | `1984` |
| Year and month | `string` (pattern:`/[0-9]{4}-[0-9]{2}/)` | `1984-01` |
| Full date without time | `date` | `1984-01-22` |
| Date and time | `date-time` | `1984-01-22T01:23:45.678Z` |

## See Also

### Filtering by Release Date

object DateComponentsRange

A period of time from a specified start date to a specified end date.

object ExplicitDateComponents

A date or time in specified of units (such as year, month, day, hour, and minute) for evaluation in a calendar system and time zone.

