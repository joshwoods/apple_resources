

- Core Motion
- CMPedometerData
-  floorsAscended 

Instance Property

# floorsAscended

The approximate number of floors ascended by walking.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
var floorsAscended: NSNumber? { get }
```

## Discussion

This value reflects only the floors ascended while the user was walking or running up stairs and does not reflect the floors ascended by elevator or other assisted means. A single floor has a height of approximately three meters. The value in this property is `nil` when floor counting is not supported on the current device.

## See Also

### Getting the Floor Counts

var floorsDescended: NSNumber?

The approximate number of floors descended by walking.

