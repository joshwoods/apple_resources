

- ClockKit
- CLKComplicationDescriptor
-  identifier 

Instance Property

# identifier

A string that uniquely identifies the descriptor.

watchOS 7.0+

``` source
var identifier: String { get }
```

## See Also

### Accessing the descriptor’s data

var displayName: String

A localized string that identifies complications from the descriptor to the user.

var supportedFamilies: [CLKComplicationFamily]

The families that support this type of complication.

var userActivity: NSUserActivity?

A user activity object that represents the state of the app at a moment in time.

var userInfo: [AnyHashable : Any]?

A dictionary of data that your data source can use to generate timeline entries.

