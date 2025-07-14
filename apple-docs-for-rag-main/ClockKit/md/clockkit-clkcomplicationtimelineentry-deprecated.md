

- ClockKit
-  CLKComplicationTimelineEntry Deprecated

Class

# CLKComplicationTimelineEntry

A container for the complication template object to display and the time to display it.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTimelineEntry
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Overview

Each entry object represents a single data point along your complication’s timeline. You create and return timeline entries when asked to do so by ClockKit. When the date associated with a particular timeline entry occurs, ClockKit updates your complication’s interface with the data in the accompanying template object.

You can assign a group identifier to timeline entries to control the behavior of transition animations during Time Travel. When two timeline entries have different values in their timelineAnimationGroup property, or when the values are `nil`, ClockKit animates the transition between those entries during Time Travel. When two entries have the same group value, no animation is created.

## Topics

### Creating a Timeline Entry

convenience init(date: Date, complicationTemplate: CLKComplicationTemplate)

Creates and returns a timeline entry with the specified date and complication data.

convenience init(date: Date, complicationTemplate: CLKComplicationTemplate, timelineAnimationGroup: String?)

Creates and returns a timeline entry with the specified information.

### Setting the Entry Values

var date: Date

The time at which to display the entry.

var complicationTemplate: CLKComplicationTemplate

The template containing the data to display in your complication.

var timelineAnimationGroup: String?

The animation group to which the entry belongs.

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

class CLKComplicationServer

An object that manages the active complications for an app.

Deprecated

class CLKComplication

Metadata about a custom complication.

Deprecated

