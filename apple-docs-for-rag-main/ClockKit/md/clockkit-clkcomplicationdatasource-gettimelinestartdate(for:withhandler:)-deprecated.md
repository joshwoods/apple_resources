

- ClockKit
- CLKComplicationDataSource
-  getTimelineStartDate(for:withHandler:) Deprecated

Instance Method

# getTimelineStartDate(for:withHandler:)

Retrieves the earliest date for which your complication is prepared to supply data.

watchOS 2.0–7.0Deprecated

``` source
@MainActor
optional func getTimelineStartDate(
    for complication: CLKComplication,
    withHandler handler: @escaping (Date?) -> Void
)
```

Deprecated

Time Travel and backwards extension of timelines are no longer supported.

## Parameters 

`complication`  

The complication tied to the request.

`handler`  

The handler to execute with the start date. This block has no return value and takes the following parameter:

`date`  
The start date for your data. For times before this date, WatchKit dims your data to indicate that the timeline doesn’t continue. If you specify `nil`, ClockKit doesn’t ask for any more past data.

## Discussion

Only implement this method if your app supports Time Travel on watchOS 4 or earlier.

Your implementation of this method must execute the block in the `handler` parameter and specify the earliest date for which you can supply timeline entries. If you don’t support displaying past data using Time Travel, specify the current date.

If you don’t implement this method, ClockKit doesn’t attempt to retrieve timeline entries before the current entry.

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

func getSupportedTimeTravelDirections(for: CLKComplication, withHandler: (CLKComplicationTimeTravelDirections) -> Void)

Determines whether your complication can provide timeline entries for the future or the past.

Deprecated

struct CLKComplicationTimeTravelDirections

Constants indicating the supported time travel directions, if any.

Deprecated

