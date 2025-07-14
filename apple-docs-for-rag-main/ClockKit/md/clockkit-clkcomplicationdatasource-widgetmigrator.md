

- ClockKit
- CLKComplicationDataSource
-  widgetMigrator 

Instance Property

# widgetMigrator

A migrator that maps ClockKit complications to their WidgetKit replacements.

watchOS 9.0+

``` source
@MainActor
optional var widgetMigrator: any CLKComplicationWidgetMigrator { get }
```

## Discussion

Implement this to provide an instance that can migrate a user’s ClockKit complications to their WidgetKit replacements. For example, update your data source so that it also conforms to the CLKComplicationWidgetMigrator protocol.

```
class ComplicationController: NSObject, CLKComplicationDataSource, CLKComplicationWidgetMigrator {
   // ...
}
```

Then, have its widgetMigrator property return `self`.

```
var widgetMigrator: CLKComplicationWidgetMigrator {
    self
}
```

Finally, implement the getWidgetConfiguration(from:completionHandler:) method. This method determines the best WidgetKit configuration for the given complication descriptor. The following example uses the Swift async version of the method.

```
func widgetConfiguration(from complicationDescriptor: CLKComplicationDescriptor) async -> CLKComplicationWidgetMigrationConfiguration? {

    switch complicationDescriptor.identifier {
    case caffeineDoseIdentifier:
        return CLKComplicationStaticWidgetMigrationConfiguration(
            kind: "Caffeine_Complications",
            extensionBundleIdentifier: "com.example.apple-samplecode.Coffee-Tracker.watchkitapp.watchkitextension.CoffeeTracker-Complications")

    case cupTotalIdentifier:
        return CLKComplicationStaticWidgetMigrationConfiguration(
            kind: "CupTotal_Complications",
            extensionBundleIdentifier: "com.example.apple-samplecode.Coffee-Tracker.watchkitapp.watchkitextension.CoffeeTracker-Complications")

    case cupAndCaffeineIdentifier:
        return CLKComplicationStaticWidgetMigrationConfiguration(
            kind: "CupAndCaffeine_Complications",
            extensionBundleIdentifier: "com.example.apple-samplecode.Coffee-Tracker.watchkitapp.watchkitextension.CoffeeTracker-Complications")

    default:
        return nil
    }
}
```

## See Also

### Migrating to WidgetKit

class CLKComplicationStaticWidgetMigrationConfiguration

A configuration object that specifies a static complication in WidgetKit.

class CLKComplicationAppIntentWidgetMigrationConfiguration

A configuration object that specifies a WidgetKit complication that uses app intents.

class CLKComplicationIntentWidgetMigrationConfiguration

A configuration object that specifies an intents-based complication in WidgetKit.

protocol CLKComplicationWidgetMigrator

A protocol that maps ClockKit complications to their WidgetKit replacements.

class CLKComplicationWidgetMigrationConfiguration

An abstract class that specifies WidgetKit complications.

