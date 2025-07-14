

- ClockKit
- CLKComplicationDataSource
-  getTimelineEntries(for:before:limit:withHandler:) Deprecated

Instance Method

# getTimelineEntries(for:before:limit:withHandler:)

Retrieves past timeline entries for the complication.

watchOS 2.0–7.0Deprecated

``` source
@MainActor
optional func getTimelineEntries(
    for complication: CLKComplication,
    before date: Date,
    limit: Int,
    withHandler handler: @escaping ([CLKComplicationTimelineEntry]?) -> Void
)
```

Deprecated

Time Travel and backwards extension of timelines are no longer supported.

## Parameters 

`complication`  

The complication tied to the request. Use the complication family information in this object to determine which set of templates are valid.

`date`  

The end date for providing past entries. The dates for your timeline entries should occur before this date and be as close to the date as possible.

`limit`  

The maximum number of entries to provide.

`handler`  

The handler to execute with the past timeline data. This block has no return value and takes the following parameter:

`entries`  
An array of CLKComplicationTimelineEntry objects representing the past data. The number of entries in the array must be less than or equal to the value in the `limit` parameter. If you specify `nil`, ClockKit doesn’t try to extend the timeline further.

## Discussion

Only implement this method if your app supports Time Travel on watchOS 4 or earlier.

Use this method to build an array of timeline entries with your app’s past data. Each timeline entry contains the data and the date at which that data is valid. Don’t provide entries with dates after the one in the `date` parameter, and limit the number of entries you create to the value in the `limit` parameter.

The array you return must start in the past and extend forward into time, ending no later than the date specified in the `date` parameter. Each successive entry in the array must come after the one before it. Entries must be greater than one minute apart. If two entries are less than one minute apart, ClockKit discards one of the entries.

Don’t include the current entry in your array. That entry is retrieved separately using the getCurrentTimelineEntry(for:withHandler:) method.

If you don’t implement this method, ClockKit doesn’t try to add earlier entries to the timeline.

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

