

- ClockKit
- CLKComplicationDataSource
-  getNextRequestedUpdateDate(handler:) Deprecated

Instance Method

# getNextRequestedUpdateDate(handler:)

Gets the next time at which to update your complication.

watchOS 2.0–4.0Deprecated

``` source
@MainActor
optional func getNextRequestedUpdateDate(handler: @escaping (Date?) -> Void)
```

Deprecated

Use WKRefreshBackgroundTask instead.

## Parameters 

`handler`  

The handler to execute with the next date at which to run your complication code. This block has no return value and takes the following parameter:

`updateDate`  
The date after which you’d like your complication to run again. If you specify `nil`, ClockKit doesn’t schedule a new update time for your complication. You can still trigger updates manually.

## Discussion

Your implementation of this method must execute the block in the `handler` parameter and specify an appropriate date. Specify a date as far into the future as you can manage for your complications. ClockKit wakes up your complication at some point after the specified date to request new data. The exact time at which your complication runs isn’t guaranteed.

If your complication data changes before the specified update date, you can invalidate your complication data using the CLKComplicationServer object.

If you don’t implement this method, ClockKit doesn’t schedule your complication for another update. You must trigger updates to your complication’s data manually by extending or reloading your timeline.

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

