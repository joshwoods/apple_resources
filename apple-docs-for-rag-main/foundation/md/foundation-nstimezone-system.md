

- Foundation
- NSTimeZone
-  system 

Type Property

# system

The time zone currently used by the system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var system: TimeZone { get }
```

## Discussion

If the current system time zone cannot be determined, the GMT time zone is used instead.

If you access the system class property, its value is cached by the app and doesn’t update if the user subsequently changes the system time zone. In order for the system property to reflect the new time zone, you must first call the resetSystemTimeZone() method to clear the cached value. Then, the next time you access the system property, it returns the current system time zone, and caches that value.

If you access the system class property, assign its value to a variable, and clear the cached value for the property by calling the resetSystemTimeZone() method, the object stored in the variable doesn’t update to reflect the new system time zone. Contrast this behavior with that of the local class property, which returns a proxy object that always reflects the current system time zone.

## See Also

### Working with System Time Zones

class var local: TimeZone

An object that tracks the current system time zone.

class func resetSystemTimeZone()

Clears any time zone value cached for the system property.

class var `default`: TimeZone

The default time zone for the current app.

