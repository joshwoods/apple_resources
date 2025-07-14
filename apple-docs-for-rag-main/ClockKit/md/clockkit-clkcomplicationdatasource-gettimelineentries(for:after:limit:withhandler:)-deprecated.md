

- ClockKit
- CLKComplicationDataSource
-  getTimelineEntries(for:after:limit:withHandler:) Deprecated

Instance Method

# getTimelineEntries(for:after:limit:withHandler:)

Retrieves future timeline entries for the complication.

watchOS 2.0–9.0Deprecated

``` source
@MainActor
optional func getTimelineEntries(
    for complication: CLKComplication,
    after date: Date,
    limit: Int,
    withHandler handler: @escaping ([CLKComplicationTimelineEntry]?) -> Void
)
```

``` source
@MainActor
optional func timelineEntries(
    for complication: CLKComplication,
    after date: Date,
    limit: Int
) async -> [CLKComplicationTimelineEntry]?
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Parameters 

`complication`  

The complication tied to the request. Use the complication family information in this object to determine which set of templates are valid.

`date`  

The starting date for providing future entries. The dates for your timeline entries should occur after this date and be as close to the date as possible.

`limit`  

The maximum number of entries to provide.

`handler`  

The handler to execute with the future timeline data. This block has no return value and takes the following parameter:

`entries`  
An array of CLKComplicationTimelineEntry objects representing the future data. The number of entries in the array must be less than or equal to the value in the `limit` parameter. If you specify `nil`, ClockKit doesn’t try to extend the timeline further.

## Mentioned in 

Sharing an Apple Watch face

Loading future timeline events

## Discussion

Use this method to build an array of timeline entries with your app’s future data. Each timeline entry contains the data and the date at which that data is valid. Don’t provide entries that occur before the date in the `date` parameter, and limit the number of entries you create to the value in the `limit` parameter.

The array you return must start after the date specified in the `date` parameter and extend forward in time. Each successive entry in the array must come after the one before it. Entries must be greater than one minute apart. If two entries are less than one minute apart, ClockKit discards one of the entries.

Don’t include the current entry in your array. That entry is retrieved separately using the getCurrentTimelineEntry(for:withHandler:) method.

If you don’t implement this method, ClockKit doesn’t try to add later entries to the timeline.

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

