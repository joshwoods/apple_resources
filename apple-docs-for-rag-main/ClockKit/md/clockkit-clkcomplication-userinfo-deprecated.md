

- ClockKit
- CLKComplication
-  userInfo Deprecated

Instance Property

# userInfo

A dictionary of additional data associated with the complication.

watchOS 7.0–9.0Deprecated

``` source
var userInfo: [AnyHashable : Any]? { get }
```

## Mentioned in 

Creating a timeline entry

Sharing an Apple Watch face

## Discussion

Because the system can pass configurations as part of a shared watch face, only include data in the user info dictionary that any instance of the app can use. For example, avoid using identifiers that might change between users, like an index into the user’s favorites list. Instead, use items that remain constant across all copies of the app, like unique string identifiers.

When the user taps your complication, ClockKit includes the content of the `userInfo` property in the dictionary passed to the extension delegate’s handleUserActivity(_:) method. Your data source can also access the user info dictionary when creating the template for this complication.

## See Also

### Accessing Data About the Complication

var family: CLKComplicationFamily

The family to which the complication belongs.

Deprecated

var identifier: String

An identifier that specifies a complication if your app supports multiple complications per family.

Deprecated

var userActivity: NSUserActivity?

An object that represents the state of the app at a moment in time.

Deprecated

