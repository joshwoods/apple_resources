

- ClockKit
- CLKComplicationDataSource
-  getPrivacyBehavior(for:withHandler:) Deprecated

Instance Method

# getPrivacyBehavior(for:withHandler:)

Returns the privacy behavior for the specified complication.

watchOS 2.0–9.0Deprecated

``` source
@MainActor
optional func getPrivacyBehavior(
    for complication: CLKComplication,
    withHandler handler: @escaping (CLKComplicationPrivacyBehavior) -> Void
)
```

``` source
@MainActor
optional func privacyBehavior(for complication: CLKComplication) async -> CLKComplicationPrivacyBehavior
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Parameters 

`complication`  

The complication tied to the request.

`handler`  

The handler to execute with the privacy behavior. This block has no return value and takes the following parameter:

behavior  
The privacy behavior to apply to the specified complication. You can specify different privacy behaviors for different complication families.

## Discussion

ClockKit calls this method to determine how to display your complication data when the user’s Apple Watch is locked. If your complication contains any personal information for the user, pass the CLKComplicationPrivacyBehavior.hideOnLockScreen value to the handler. For data that’s already available publicly, you may pass the CLKComplicationPrivacyBehavior.showOnLockScreen value to the handler to allow that data to be displayed.

If you don’t implement this method, ClockKit uses the value CLKComplicationPrivacyBehavior.showOnLockScreen as the default.

## Topics

### Privacy Behaviors

enum CLKComplicationPrivacyBehavior

Constants indicating the complication behavior when the Apple Watch is locked.

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

