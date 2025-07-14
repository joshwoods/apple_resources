

- ClockKit
- CLKComplicationDescriptor
-  userActivity 

Instance Property

# userActivity

A user activity object that represents the state of the app at a moment in time.

watchOS 7.0+

``` source
var userActivity: NSUserActivity? { get }
```

## Discussion

When the user taps on a complication specified by this configuration, the system launches the app and calls handle(_:), passing the user activity. Your extension delegate’s handle method should update the app so that it’s in the specified state.

Because the system can pass configurations as part of a shared watch face, only include data useable by any instance of the app. For example, avoid using identifiers that might change between users, like an index into the user’s favorites list. Instead, use items that remain constant across all copies of the app, like unique string identifiers.

## See Also

### Accessing the descriptor’s data

var identifier: String

A string that uniquely identifies the descriptor.

var displayName: String

A localized string that identifies complications from the descriptor to the user.

var supportedFamilies: [CLKComplicationFamily]

The families that support this type of complication.

var userInfo: [AnyHashable : Any]?

A dictionary of data that your data source can use to generate timeline entries.

