

- Foundation
- NSLocale
-  currentLocaleDidChangeNotification 

Type Property

# currentLocaleDidChangeNotification

A notification that indicates that the user’s locale changed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let currentLocaleDidChangeNotification: NSNotification.Name
```

## Discussion

Register for this notification if your app displays content (dates, times, numbers, and so on) that is affected by the locale. Use the notification to trigger updates to your app’s interface.

## See Also

### Related Documentation

class NSNotification

A container for information broadcast through a notification center to all registered observers.

### Getting the User’s Locale

class var autoupdatingCurrent: Locale

A locale which tracks the user’s current preferences.

class var current: Locale

A locale representing the user’s region settings at the time the property is read.

class var system: Locale

A locale representing the generic root values with little localization.

