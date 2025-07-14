

- ClockKit
- CLKComplicationDescriptor
-  supportedFamilies 

Instance Property

# supportedFamilies

The families that support this type of complication.

watchOS 7.0+

``` source
var supportedFamilies: [CLKComplicationFamily] { get }
```

## Discussion

Different descriptors can support different sets of families.

## See Also

### Accessing the descriptor’s data

var identifier: String

A string that uniquely identifies the descriptor.

var displayName: String

A localized string that identifies complications from the descriptor to the user.

var userActivity: NSUserActivity?

A user activity object that represents the state of the app at a moment in time.

var userInfo: [AnyHashable : Any]?

A dictionary of data that your data source can use to generate timeline entries.

