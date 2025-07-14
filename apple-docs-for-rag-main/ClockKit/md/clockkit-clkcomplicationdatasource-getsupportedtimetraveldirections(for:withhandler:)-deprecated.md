

- ClockKit
- CLKComplicationDataSource
-  getSupportedTimeTravelDirections(for:withHandler:) Deprecated

Instance Method

# getSupportedTimeTravelDirections(for:withHandler:)

Determines whether your complication can provide timeline entries for the future or the past.

watchOS 2.0–7.0Deprecated

``` source
@MainActor
optional func getSupportedTimeTravelDirections(
    for complication: CLKComplication,
    withHandler handler: @escaping (CLKComplicationTimeTravelDirections) -> Void
)
```

Deprecated

Time Travel is no longer supported. Use CLKComplicationDataSource's getTimelineEndDateForComplication:withHandler: to specify forward timeline support.

## Parameters 

`complication`  

The complication tied to the request.

`handler`  

The handler to execute with the Time Travel directions. This block has no return value and takes the following parameter:

directions  
The supported time travel directions. You may combine the values of the CLKComplicationTimeTravelDirections type when specifying this value.

## Mentioned in 

Loading future timeline events

## Discussion

The system calls this method to determine whether your app can provide future or past data entries for the specified complication type. Your implementation of this method must execute the block in the `handler` parameter and specify the supported directions.

Include the backward constant if your app provides a historical record of events that have occurred or information that was valid at specific times. For example, a music app could provide entries for songs that have already played.

Include the forward constant if your app is able to generate complication data tied to future dates. For example, a calendar app would provide entries for future meeting times.

In watchOS 7 and later, the system checks the value returned by getTimelineEndDate(for:withHandler:) instead. If the method returns a non-nil value, ClockKit attempts to bulk load future timeline entries. Otherwise, it only asks for the current timeline entry.

## Topics

### Time Travel Directions

struct CLKComplicationTimeTravelDirections

Constants indicating the supported time travel directions, if any.

## See Also

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

struct CLKComplicationTimeTravelDirections

Constants indicating the supported time travel directions, if any.

Deprecated

func getTimelineStartDate(for: CLKComplication, withHandler: (Date?) -> Void)

Retrieves the earliest date for which your complication is prepared to supply data.

Deprecated

