

- ClockKit
-  CLKComplicationStaticWidgetMigrationConfiguration 

Class

# CLKComplicationStaticWidgetMigrationConfiguration

A configuration object that specifies a static complication in WidgetKit.

watchOS 9.0+

``` source
class CLKComplicationStaticWidgetMigrationConfiguration
```

## Overview

You can use static complications if your app doesn’t dynamically customize the list of complications available in the complication picker. For example, if your complications display the current temperature and chance of precipitation at the user’s current location, you can use a set of static widgets to define these complications.

For more information, see Migrating ClockKit complications to WidgetKit.

## Topics

### Creating static complication configurations

init(kind: String, extensionBundleIdentifier: String)

Creates an object that describes a static watchOS complication in your WidgetKit extension.

### Accessing configuration properties

var kind: String

A string that uniquely identifies a widget in your WidgetKit extension.

var extensionBundleIdentifier: String

The bundle identifier for your WidgetKit extension.

## Relationships

### Inherits From

- CLKComplicationWidgetMigrationConfiguration

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

class CLKComplicationAppIntentWidgetMigrationConfiguration

A configuration object that specifies a WidgetKit complication that uses app intents.

class CLKComplicationIntentWidgetMigrationConfiguration

A configuration object that specifies an intents-based complication in WidgetKit.

protocol CLKComplicationWidgetMigrator

A protocol that maps ClockKit complications to their WidgetKit replacements.

class CLKComplicationWidgetMigrationConfiguration

An abstract class that specifies WidgetKit complications.

