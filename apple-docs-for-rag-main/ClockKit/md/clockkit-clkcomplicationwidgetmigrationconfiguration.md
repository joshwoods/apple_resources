

- ClockKit
-  CLKComplicationWidgetMigrationConfiguration 

Class

# CLKComplicationWidgetMigrationConfiguration

An abstract class that specifies WidgetKit complications.

watchOS 9.0+

``` source
class CLKComplicationWidgetMigrationConfiguration
```

## Overview

The CLKComplicationWidgetMigrationConfiguration class is the basis for all classes that describe watchOS complications in WidgetKit. Because it’s an abstract class, you don’t instantiate it directly. Instead, create one of its concrete subclasses: CLKComplicationStaticWidgetMigrationConfiguration, CLKComplicationAppIntentWidgetMigrationConfiguration, or CLKComplicationIntentWidgetMigrationConfiguration.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CLKComplicationAppIntentWidgetMigrationConfiguration
- CLKComplicationIntentWidgetMigrationConfiguration
- CLKComplicationStaticWidgetMigrationConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
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

protocol CLKComplicationWidgetMigrator

A protocol that maps ClockKit complications to their WidgetKit replacements.

