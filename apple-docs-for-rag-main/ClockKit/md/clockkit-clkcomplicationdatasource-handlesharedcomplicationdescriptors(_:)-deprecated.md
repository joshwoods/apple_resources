

- ClockKit
- CLKComplicationDataSource
-  handleSharedComplicationDescriptors(\_:) Deprecated

Instance Method

# handleSharedComplicationDescriptors(\_:)

Informs the app about complications from a shared watch face.

watchOS 7.0–9.0Deprecated

``` source
@MainActor
optional func handleSharedComplicationDescriptors(_ complicationDescriptors: [CLKComplicationDescriptor])
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Parameters 

`complicationDescriptors`  

The descriptors for your app’s complications from a shared watch face.

## Mentioned in 

Sharing an Apple Watch face

## Discussion

ClockKit calls this method when the Apple Watch receives a shared watch face that contains one or more of your app’s complications. Implement this method to prepare your app so that it can provide complication data for the descriptors.

For example, a weather app may provide separate complications for all of the user’s favorite cities. However, when the user receives a shared watch face from someone else, the shared watch face may include a complication for a city that isn’t in the user’s favorite city list. The weather app needs to provide data for the new city, and may need to add the city to the user’s favorite list.

```
func handleSharedComplicationDescriptors(_ complicationDescriptors: [CLKComplicationDescriptor]) {
    // If the descriptor has a city ID, add it to the favorite city list,
    // so the app will download weather updates for the city.
    for descriptor in complicationDescriptors {
        guard let cityID = descriptor.userInfo?[myCityIDKey] as? String else { continue }
        myData.addFavoriteCity(byID: cityID)
    }
}
```

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

