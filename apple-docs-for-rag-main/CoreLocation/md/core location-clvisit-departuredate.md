

- Core Location
- CLVisit
-  departureDate 

Instance Property

# departureDate

The approximate time at which the user left the specified location.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+

``` source
var departureDate: Date { get }
```

## Discussion

When the visit object does not include departure information, this property is set to the date returned by the distantFuture method of NSDate.

## See Also

### Getting the visit duration

var arrivalDate: Date

The approximate time at which the user arrived at the specified location.

