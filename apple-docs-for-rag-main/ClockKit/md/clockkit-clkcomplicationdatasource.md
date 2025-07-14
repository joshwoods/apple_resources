

- ClockKit
-  CLKComplicationDataSource 

Protocol

# CLKComplicationDataSource

A protocol that provides ClockKit with information about your complication.

watchOS 2.0+

``` source
@MainActor
protocol CLKComplicationDataSource : NSObjectProtocol
```

## Mentioned in 

Sharing an Apple Watch face

Enabling Complications for Your watchOS App

## Overview

Apps that support a complication must define a class that supports the CLKComplicationDataSource protocol and register it with the system. Your data source is responsible for providing timeline entries and data for all of the complication families that you support. You do this by implementing the protocol methods, returning the timeline entries displayed by your complication and information about the features that your complication supports.

You don’t instantiate your data source class explicitly. After defining your class, specify the class name in the General tab of the project settings for your WatchKit extension. When the system needs data, ClockKit instantiates your data source and initializes it by calling its `init` method. Once initialized, ClockKit calls the corresponding protocol methods to gather any needed data. You can also specify your class name in your app’s `Info.plist` file using the `CLKComplicationsPrincipalClass` key.

When the user installs your complication on the clock face, ClockKit creates an appropriate CLKComplication object for the selected complication family. ClockKit then passes the complication to your data source so that you know how to format your timeline entries. Use the General tab of your WatchKit extension’s project settings to specify the families you support.

Your complication data source class must implement the CLKComplicationDataSource protocol’s getCurrentTimelineEntry(for:withHandler:) method.

You may implement other methods as needed to support the data in your complication. For example, to batch load future timeline entries, implement getTimelineEndDate(for:withHandler:) and pass a future date to the handler. For more information, see Creating complications for your watchOS app.

Note

For watchOS 6 and earlier, you must implement both getCurrentTimelineEntry(for:withHandler:) and getSupportedTimeTravelDirections(for:withHandler:). Use getSupportedTimeTravelDirections(for:withHandler:) to specify whether your app can batch load future timeline entries.

ClockKit calls your data source methods on your watchOS app’s main thread.

## Topics

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

class CLKComplicationWidgetMigrationConfiguration

An abstract class that specifies WidgetKit complications.

### Setting information property keys

CLKComplicationPrincipalClass

The name of the class that implements the complication data source protocol.

### Deprecated methods

let CLKLaunchedTimelineEntryDateKey: String

A key that indicates the date when the system launched the complication.

Deprecated

let CLKLaunchedComplicationIdentifierKey: String

A key that indicates the identifier of a complication the system launched.

Deprecated

func getComplicationDescriptors(handler: ([CLKComplicationDescriptor]) -> Void)

Returns the list of complication descriptors.

Deprecated

func handleSharedComplicationDescriptors([CLKComplicationDescriptor])

Informs the app about complications from a shared watch face.

Deprecated

func getLocalizableSampleTemplate(for: CLKComplication, withHandler: (CLKComplicationTemplate?) -> Void)

Gets a localizable template that shows sample data for the specified complication.

Deprecated

func getPrivacyBehavior(for: CLKComplication, withHandler: (CLKComplicationPrivacyBehavior) -> Void)

Returns the privacy behavior for the specified complication.

Deprecated

enum CLKComplicationPrivacyBehavior

Constants indicating the complication behavior when the Apple Watch is locked.

Deprecated

func getAlwaysOnTemplate(for: CLKComplication, withHandler: (CLKComplicationTemplate?) -> Void)

Returns the template to use during Always On.

Deprecated

func getTimelineEndDate(for: CLKComplication, withHandler: (Date?) -> Void)

Retrieves the last date for the data that your app can supply.

Deprecated

func getCurrentTimelineEntry(for: CLKComplication, withHandler: (CLKComplicationTimelineEntry?) -> Void)

Retrieves the timeline entry that you want to display now.

**Required**

Deprecated

func getTimelineEntries(for: CLKComplication, after: Date, limit: Int, withHandler: ([CLKComplicationTimelineEntry]?) -> Void)

Retrieves future timeline entries for the complication.

Deprecated

func getTimelineAnimationBehavior(for: CLKComplication, withHandler: (CLKComplicationTimelineAnimationBehavior) -> Void)

Gets the animation behavior when transitioning between timeline entries.

Deprecated

enum CLKComplicationTimelineAnimationBehavior

Constants indicating the animation behavior during Time Travel.

Deprecated

func getSupportedTimeTravelDirections(for: CLKComplication, withHandler: (CLKComplicationTimeTravelDirections) -> Void)

Determines whether your complication can provide timeline entries for the future or the past.

Deprecated

struct CLKComplicationTimeTravelDirections

Constants indicating the supported time travel directions, if any.

Deprecated

func getTimelineStartDate(for: CLKComplication, withHandler: (Date?) -> Void)

Retrieves the earliest date for which your complication is prepared to supply data.

Deprecated

func getTimelineEntries(for: CLKComplication, before: Date, limit: Int, withHandler: ([CLKComplicationTimelineEntry]?) -> Void)

Retrieves past timeline entries for the complication.

Deprecated

func getNextRequestedUpdateDate(handler: (Date?) -> Void)

Gets the next time at which to update your complication.

Deprecated

func requestedUpdateDidBegin()

Indicates that a requested update has begun so that you’ve an opportunity to extend or reload your timeline.

Deprecated

func requestedUpdateBudgetExhausted()

Indicates that your complication’s time budget is exhausted.

Deprecated

func getPlaceholderTemplate(for: CLKComplication, withHandler: (CLKComplicationTemplate?) -> Void)

Gets a static template to display in the selection screen for your complication.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Migration Support

Migrating ClockKit complications to WidgetKit

Leverage WidgetKit’s API to create watchOS complications using SwiftUI.

let CLKDefaultComplicationIdentifier: String

An identifier representing a default complication.

class CLKComplicationDescriptor

A descriptor that defines a complication and the families that it supports.

