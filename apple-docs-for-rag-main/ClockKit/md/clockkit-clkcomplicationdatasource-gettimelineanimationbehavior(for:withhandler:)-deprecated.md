

- ClockKit
- CLKComplicationDataSource
-  getTimelineAnimationBehavior(for:withHandler:) Deprecated

Instance Method

# getTimelineAnimationBehavior(for:withHandler:)

Gets the animation behavior when transitioning between timeline entries.

watchOS 2.0–9.0Deprecated

``` source
@MainActor
optional func getTimelineAnimationBehavior(
    for complication: CLKComplication,
    withHandler handler: @escaping (CLKComplicationTimelineAnimationBehavior) -> Void
)
```

``` source
@MainActor
optional func timelineAnimationBehavior(for complication: CLKComplication) async -> CLKComplicationTimelineAnimationBehavior
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Parameters 

`complication`  

The complication tied to the request. Use the complication family information in this object to determine which set of templates are valid.

`handler`  

The handler to execute with the animation behavior. This block has no return value and takes the following parameter:

behavior  
The animation behavior to use. For a list of possible values, see CLKComplicationTimelineAnimationBehavior.

## Discussion

Only implement this method if your app supports Time Travel on watchOS 4 or earlier.

Implement this method if you want ClockKit to create transition animations between your timeline entries during Time Travel. Transition animations create softer transitions between different entries. You might use them when the value of an entry changes dramatically or when you change the template you’re using.

You can use group identifiers to eliminate transition animations between specific timeline entries. When animations are enabled, ClockKit creates animations only when the group identifier of successive timeline entries is different.

If you don’t implement this method, ClockKit doesn’t animate the transitions between timeline entries.

## Topics

### Animation Behaviors

enum CLKComplicationTimelineAnimationBehavior

Constants indicating the animation behavior during Time Travel.

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

