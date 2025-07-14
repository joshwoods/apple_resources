

- Core Motion
- CMPedometerData
-  floorsDescended 

Instance Property

# floorsDescended

The approximate number of floors descended by walking.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
var floorsDescended: NSNumber? { get }
```

## Discussion

This value reflects only the floors descended while the user was walking or running down stairs and does not reflect the floors descended by elevator or other assisted means. A single floor has a height of approximately three meters. The value in this property is `nil` when floor counting is not supported on the current device.

## See Also

### Getting the Floor Counts

var floorsAscended: NSNumber?

The approximate number of floors ascended by walking.

