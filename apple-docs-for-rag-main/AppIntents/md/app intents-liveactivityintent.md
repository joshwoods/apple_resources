

- App Intents
-  LiveActivityIntent 

Protocol

# LiveActivityIntent

An intent that starts, pauses, or otherwise modifies a Live Activity when it runs.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
protocol LiveActivityIntent : SystemIntent
```

## Overview

To gain permission for starting Live Activities, conform to this protocol. Create and start a Live Activity manually in your perform() method. For more information, see the ActivityKit framework.

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable
- SystemIntent

## See Also

### Controls, widgets, and Live Activities

protocol ControlConfigurationIntent

An interface for configuring a Control Center module.

protocol LiveActivityStartingIntent

An intent that starts, pauses, or otherwise modifies a Live Activity.

Deprecated

protocol WidgetConfigurationIntent

An interface for configuring a WidgetKit widget.

