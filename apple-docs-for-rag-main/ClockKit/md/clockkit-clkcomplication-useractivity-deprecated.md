

- ClockKit
- CLKComplication
-  userActivity Deprecated

Instance Property

# userActivity

An object that represents the state of the app at a moment in time.

watchOS 7.0–9.0Deprecated

``` source
var userActivity: NSUserActivity? { get }
```

## Mentioned in 

Sharing an Apple Watch face

## Discussion

When the user taps on a complication specified by this configuration, the system launches the app and calls handle(_:), passing the user activity. Your extension delegate’s handle(_:) method should update the app so that it’s in the specified state.

Because the system can pass configurations as part of a shared watch face, only include data useable by any instance of the app. For example, avoid using identifiers that might change between users, like an index into the user’s favorites list. Instead, use items that remain constant across all copies of the app, like unique string identifiers.

## See Also

### Accessing Data About the Complication

var family: CLKComplicationFamily

The family to which the complication belongs.

Deprecated

var identifier: String

An identifier that specifies a complication if your app supports multiple complications per family.

Deprecated

var userInfo: [AnyHashable : Any]?

A dictionary of additional data associated with the complication.

Deprecated

