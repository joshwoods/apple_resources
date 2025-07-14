

- Foundation
- NSTimeZone
-  default 

Type Property

# default

The default time zone for the current app.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var `default`: TimeZone { get set }
```

## Discussion

If no default time zone has been set, the current system time zone is used. If the current system time zone cannot be determined, the GMT time zone is used instead.

The default time zone is used by the app for date and time operations. You can set it to cause the app to run as if it were in a different time zone. Setting the default property clears any value that was previously set.

If you access the default class property, assign its value to a variable, and set a new default time zone, the object stored in the variable doesn’t update to reflect the new default time zone. Contrast this behavior with that of the local class property, which returns a proxy object that always reflects the current system time zone.

## See Also

### Working with System Time Zones

class var local: TimeZone

An object that tracks the current system time zone.

class var system: TimeZone

The time zone currently used by the system.

class func resetSystemTimeZone()

Clears any time zone value cached for the system property.

