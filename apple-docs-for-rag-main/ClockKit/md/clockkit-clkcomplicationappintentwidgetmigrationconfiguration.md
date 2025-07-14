

- ClockKit
-  CLKComplicationAppIntentWidgetMigrationConfiguration 

Class

# CLKComplicationAppIntentWidgetMigrationConfiguration

A configuration object that specifies a WidgetKit complication that uses app intents.

watchOS 10.0+

``` source
class CLKComplicationAppIntentWidgetMigrationConfiguration where Intent : WidgetConfigurationIntent
```

## Overview

These configuration objects use app intents to provide dynamic configuration information. Use intent-based complications when your app customizes the list of complications available in the complication picker based on the state of your app. For example, if you provide temperature complications for the top cities in the user’s favorites list, use a WidgetConfigurationIntent instance to describe each city.

For more information, see Migrating ClockKit complications to WidgetKit.

## Topics

### Creating configurations

init(kind: String, extensionBundleIdentifier: String, intent: Intent, localizedDisplayName: String)

Creates an object that describes a watchOS complication that uses app intents in your WidgetKit extension.

### Accessing configuration properties

let kind: String

A string that uniquely identifies a widget in your WidgetKit extension.

let extensionBundleIdentifier: String

The bundle identifier for your WidgetKit extension.

let intent: Intent

An intent that provides additional configuration information to your WidgetKit complication.

let localizedDisplayName: String

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

class CLKComplicationIntentWidgetMigrationConfiguration

A configuration object that specifies an intents-based complication in WidgetKit.

protocol CLKComplicationWidgetMigrator

A protocol that maps ClockKit complications to their WidgetKit replacements.

class CLKComplicationWidgetMigrationConfiguration

An abstract class that specifies WidgetKit complications.

