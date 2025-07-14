

- ClockKit
- CLKComplicationDescriptor
-  userInfo 

Instance Property

# userInfo

A dictionary of data that your data source can use to generate timeline entries.

watchOS 7.0+

``` source
var userInfo: [AnyHashable : Any]? { get }
```

## Discussion

The system passes the user info dictionary to methods like your data source’s getCurrentTimelineEntry(for:withHandler:) method as part of the complication. Your data source can use the information in the user info dictionary when creating these complications.

Because the system can pass configurations as part of a shared watch face, only include data in the user info dictionary that any instance of the app can use. For example, avoid using identifiers that might change between users, like an index into the user’s favorites list. Instead, use items that remain constant across all copies of the app, like unique string identifiers.

When the user taps your complication, ClockKit includes the content of the `userInfo` property in the dictionary passed to the extension delegate’s handleUserActivity(_:) method.

## See Also

### Accessing the descriptor’s data

var identifier: String

A string that uniquely identifies the descriptor.

var displayName: String

A localized string that identifies complications from the descriptor to the user.

var supportedFamilies: [CLKComplicationFamily]

The families that support this type of complication.

var userActivity: NSUserActivity?

A user activity object that represents the state of the app at a moment in time.

