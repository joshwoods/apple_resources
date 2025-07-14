

- ClockKit
- CLKComplicationDataSource
-  getComplicationDescriptors(handler:) Deprecated

Instance Method

# getComplicationDescriptors(handler:)

Returns the list of complication descriptors.

watchOS 7.0–9.0Deprecated

``` source
@MainActor
optional func getComplicationDescriptors(handler: @escaping ([CLKComplicationDescriptor]) -> Void)
```

``` source
@MainActor
optional func complicationDescriptors() async -> [CLKComplicationDescriptor]
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Parameters 

`handler`  

In your data source’s implementation, call the handler and pass the complication descriptors for your app. This block takes the following parameter:

`descriptors`  
An array containing your app’s complication descriptors.

## Mentioned in 

Declaring complications for your app

## Discussion

ClockKit calls this method to determine the complications that an app supports. Implement this method to define your app’s complications. For example, a weather app may support different complications for the current condition, temperature, or chance of precipitation.

You can also use your implementation to customize the types of complications according to your app’s current data. For example, a weather app could provide separate complications for the user’s favorite locations.

In your data source’s implementation, create an array of CLKComplicationDescriptor objects to represent the complications that your app supports, and then pass the array to the method’s handler.

```
```

In addition to defining a unique type of complication, each descriptor also defines the families that the complication supports. Each descriptor appears as a separate complication on the Apple Watch’s face customization screen.

The complications appear in the same order as the descriptor array. When the user configures a complication, the picker shows the first three items from the array that support the complication’s family. If there are more than three, the picker displays a More button to provide access to the additional complications.

To update the descriptors, call reloadComplicationDescriptors().

## See Also

### Deprecated methods

let CLKLaunchedTimelineEntryDateKey: String

A key that indicates the date when the system launched the complication.

Deprecated

let CLKLaunchedComplicationIdentifierKey: String

A key that indicates the identifier of a complication the system launched.

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

