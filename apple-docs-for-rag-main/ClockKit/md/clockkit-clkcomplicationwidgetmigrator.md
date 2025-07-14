

- ClockKit
-  CLKComplicationWidgetMigrator 

Protocol

# CLKComplicationWidgetMigrator

A protocol that maps ClockKit complications to their WidgetKit replacements.

watchOS 9.0+

``` source
protocol CLKComplicationWidgetMigrator : NSObjectProtocol
```

## Topics

### Migrating complications

func getWidgetConfiguration(from: CLKComplicationDescriptor, completionHandler: (CLKComplicationWidgetMigrationConfiguration?) -> Void)

Returns a configuration object that defines the WidgetKit replacement for the provided ClockKit complication.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Migrating to WidgetKit

var widgetMigrator: any CLKComplicationWidgetMigrator

A migrator that maps ClockKit complications to their WidgetKit replacements.

class CLKComplicationStaticWidgetMigrationConfiguration

A configuration object that specifies a static complication in WidgetKit.

class CLKComplicationAppIntentWidgetMigrationConfiguration

A configuration object that specifies a WidgetKit complication that uses app intents.

class CLKComplicationIntentWidgetMigrationConfiguration

A configuration object that specifies an intents-based complication in WidgetKit.

class CLKComplicationWidgetMigrationConfiguration

An abstract class that specifies WidgetKit complications.

