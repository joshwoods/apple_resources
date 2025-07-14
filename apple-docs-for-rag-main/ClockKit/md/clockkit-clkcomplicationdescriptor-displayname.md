

- ClockKit
- CLKComplicationDescriptor
-  displayName 

Instance Property

# displayName

A localized string that identifies complications from the descriptor to the user.

watchOS 7.0+

``` source
var displayName: String { get }
```

## See Also

### Accessing the descriptor’s data

var identifier: String

A string that uniquely identifies the descriptor.

var supportedFamilies: [CLKComplicationFamily]

The families that support this type of complication.

var userActivity: NSUserActivity?

A user activity object that represents the state of the app at a moment in time.

var userInfo: [AnyHashable : Any]?

A dictionary of data that your data source can use to generate timeline entries.

