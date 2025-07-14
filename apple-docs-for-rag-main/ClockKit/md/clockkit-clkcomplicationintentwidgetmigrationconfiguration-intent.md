

- ClockKit
- CLKComplicationIntentWidgetMigrationConfiguration
-  intent 

Instance Property

# intent

A SiriKit intent that provides additional configuration information to your WidgetKit complication.

watchOS 9.0+

``` source
@NSCopying
var intent: INIntent { get }
```

## See Also

### Accessing configuration properties

var kind: String

A string that uniquely identifies a widget in your WidgetKit extension.

var extensionBundleIdentifier: String

The bundle identifier for your WidgetKit extension.

var localizedDisplayName: String

A localized name for the complication.

