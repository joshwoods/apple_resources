

- ClockKit
- CLKComplicationDataSource
-  getTimelineEndDate(for:withHandler:) Deprecated

Instance Method

# getTimelineEndDate(for:withHandler:)

Retrieves the last date for the data that your app can supply.

watchOS 2.0–9.0Deprecated

``` source
@MainActor
optional func getTimelineEndDate(
    for complication: CLKComplication,
    withHandler handler: @escaping (Date?) -> Void
)
```

``` source
@MainActor
optional func timelineEndDate(for complication: CLKComplication) async -> Date?
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Parameters 

`complication`  

The complication tied to the request.

`handler`  

The handler to execute with the end date. This block has no return value and takes the following parameter:

`date`  
The end date for your data. If you specify `nil`, ClockKit doesn’t ask for any more future data.

## Mentioned in 

Loading future timeline events

Sharing an Apple Watch face

## Discussion

Your implementation of this method must execute the block in the handler parameter and specify the date. If your application can’t provide future timeline entries, specify the current date.

If you don’t implement this method, ClockKit doesn’t attempt to retrieve timeline entries after the current entry.

Important

In watchOS 6 and earlier, if you passed `nil` to the completion handler, ClockKit set the timeline end date to distantFuture. In watchOS 7 and later, it assumes your app can’t provide future data, and only asks for the current timeline entry.

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

