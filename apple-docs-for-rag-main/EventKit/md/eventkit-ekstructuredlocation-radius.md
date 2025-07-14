

- EventKit
- EKStructuredLocation
-  radius 

Instance Property

# radius

A minimum distance from the core location that would trigger the alarm or reminder.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var radius: Double { get set }
```

## Discussion

To use the default radius, set this property to `0`.

## See Also

### Accessing Structured Location Properties

var title: String?

The title of the location.

var geoLocation: CLLocation?

The core location.

