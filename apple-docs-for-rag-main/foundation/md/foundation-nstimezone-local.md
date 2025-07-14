

- Foundation
- NSTimeZone
-  local 

Type Property

# local

An object that tracks the current system time zone.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var local: TimeZone { get }
```

## Discussion

Use this property when you want an object that always reflects the current system time zone. Contrast this behavior with that of the system class property, which has its value cached until you manually clear it by calling the resetSystemTimeZone() method.

Important

In macOS High Sierra and later, iOS 11 and later, tvOS 11 and later, and watchOS 4 and later, the local class property reflects the current system time zone, whereas previously it reflected the default time zone.

Although the time zone obtained here automatically updates with the system, it provides no indication when system settings change. To receive notification of time zone changes, add an observer to the NSSystemTimeZoneDidChange notification by using the addObserver(_:selector:name:object:).

## See Also

### Working with System Time Zones

class var system: TimeZone

The time zone currently used by the system.

class func resetSystemTimeZone()

Clears any time zone value cached for the system property.

class var `default`: TimeZone

The default time zone for the current app.

