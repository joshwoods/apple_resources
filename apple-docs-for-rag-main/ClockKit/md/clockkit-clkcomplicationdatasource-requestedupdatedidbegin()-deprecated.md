

- ClockKit
- CLKComplicationDataSource
-  requestedUpdateDidBegin() Deprecated

Instance Method

# requestedUpdateDidBegin()

Indicates that a requested update has begun so that you’ve an opportunity to extend or reload your timeline.

watchOS 2.0–4.0Deprecated

``` source
@MainActor
optional func requestedUpdateDidBegin()
```

Deprecated

Use WKRefreshBackgroundTask instead.

## Discussion

When the date returned by the getNextRequestedUpdateDate(handler:) method of your data source passes, ClockKit begins a scheduled update of your complication. At the start of that update, it calls this method or the requestedUpdateBudgetExhausted() method to let you know that the requested update has begun. These methods are your opportunity to tell ClockKit whether or not you’ve new data to add to your timeline.

If you’ve new data for your timeline, your implementation of this method should call the reloadTimeline(for:) or extendTimeline(for:) method of the complication server. ClockKit doesn’t ask your data source for new timeline entries unless you call one of those methods. If you do nothing or don’t implement this method, ClockKit calls only the getNextRequestedUpdateDate(handler:) of your data source to fetch a new update time.

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

