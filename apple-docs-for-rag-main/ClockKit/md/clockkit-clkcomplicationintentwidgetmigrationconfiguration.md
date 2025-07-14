

- ClockKit
-  CLKComplicationIntentWidgetMigrationConfiguration 

Class

# CLKComplicationIntentWidgetMigrationConfiguration

A configuration object that specifies an intents-based complication in WidgetKit.

watchOS 9.0+

``` source
class CLKComplicationIntentWidgetMigrationConfiguration
```

## Overview

These configuration objects use an INIntent object to provide dynamic configuration information. Use intent-based complications when your app customizes the list of complications available in the complication picker based on the state of your app. For example, if you provide temperature complications for the top cities in the user’s favorites list, use an INIntent object to describe each city.

For more information, see Migrating ClockKit complications to WidgetKit.

## Topics

### Creating Intent widget configurations

init(kind: String, extensionBundleIdentifier: String, intent: INIntent, localizedDisplayName: String)

Creates an object that describes an intents-based watchOS complication in your WidgetKit extension.

### Accessing configuration properties

var kind: String

A string that uniquely identifies a widget in your WidgetKit extension.

var extensionBundleIdentifier: String

The bundle identifier for your WidgetKit extension.

var intent: INIntent

A SiriKit intent that provides additional configuration information to your WidgetKit complication.

var localizedDisplayName: String

A localized name for the complication.

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

class CLKComplicationStaticWidgetMigrationConfiguration

A configuration object that specifies a static complication in WidgetKit.

class CLKComplicationAppIntentWidgetMigrationConfiguration

A configuration object that specifies a WidgetKit complication that uses app intents.

protocol CLKComplicationWidgetMigrator

A protocol that maps ClockKit complications to their WidgetKit replacements.

class CLKComplicationWidgetMigrationConfiguration

An abstract class that specifies WidgetKit complications.

