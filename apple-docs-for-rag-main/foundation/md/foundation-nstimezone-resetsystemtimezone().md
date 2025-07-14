

- Foundation
- NSTimeZone
-  resetSystemTimeZone() 

Type Method

# resetSystemTimeZone()

Clears any time zone value cached for the system property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func resetSystemTimeZone()
```

## Discussion

If the app has cached the system time zone by accessing the system class property, this method clears that cached value. If you subsequently access the system class property, a new time zone object is created and cached.

## See Also

### Working with System Time Zones

class var local: TimeZone

An object that tracks the current system time zone.

class var system: TimeZone

The time zone currently used by the system.

class var `default`: TimeZone

The default time zone for the current app.

