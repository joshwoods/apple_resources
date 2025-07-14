

- ClockKit
-  CLKComplicationServer Deprecated

Class

# CLKComplicationServer

An object that manages the active complications for an app.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationServer
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

Don’t create instances of this class directly. Instead, use the shared object to fetch information about your active complications and to invalidate or extend the data for a specific complication. You can also use it to get information about the minimum and maximum dates for which you need to provide data to support Time Travel.

## Topics

### Getting the Complication Server

class func sharedInstance() -> Self

Returns the shared complication server.

### Getting the Active Complications

var activeComplications: [CLKComplication]?

The active complications for the current app.

### Updating Your Timeline Data

func reloadTimeline(for: CLKComplication)

Invalidates your existing timeline data and triggers an update session to reload it.

func extendTimeline(for: CLKComplication)

Asks the system to extend the data in your complication’s timeline.

### Updating Complication Types

func reloadComplicationDescriptors()

Reloads the complication descriptors from the complication data source.

### Getting the Time Travel Boundaries

var earliestTimeTravelDate: Date

The earliest Time Travel date for which you should provide data.

var latestTimeTravelDate: Date

The latest date supported by Time Travel.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Other Symbols

class CLKComplication

Metadata about a custom complication.

Deprecated

class CLKComplicationTimelineEntry

A container for the complication template object to display and the time to display it.

Deprecated

