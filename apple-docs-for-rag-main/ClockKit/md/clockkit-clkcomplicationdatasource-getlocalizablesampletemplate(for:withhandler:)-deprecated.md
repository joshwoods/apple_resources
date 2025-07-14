

- ClockKit
- CLKComplicationDataSource
-  getLocalizableSampleTemplate(for:withHandler:) Deprecated

Instance Method

# getLocalizableSampleTemplate(for:withHandler:)

Gets a localizable template that shows sample data for the specified complication.

watchOS 3.0–9.0Deprecated

``` source
@MainActor
optional func getLocalizableSampleTemplate(
    for complication: CLKComplication,
    withHandler handler: @escaping (CLKComplicationTemplate?) -> Void
)
```

``` source
@MainActor
optional func localizableSampleTemplate(for complication: CLKComplication) async -> CLKComplicationTemplate?
```

Deprecated

Use WidgetKit to create complications. For more information, see Migrating to WidgetKit.

## Parameters 

`complication`  

The complication tied to the request. Use the complication family information in this object to determine which set of templates are valid. For example, if the complication family is CLKComplicationFamily.utilitarianLarge, you’d instantiate the CLKComplicationTemplateUtilitarianLargeFlat class for your template.

`handler`  

The handler to execute with the template. This block has no return value and takes the following parameter:

template  
The template object containing your placeholder data. The data in this template is cached and displayed for your complication.

## Mentioned in 

Adding Placeholders for Your Complication

Sharing an Apple Watch face

## Discussion

The system calls this method once per supported complication when your extension is installed, and the results are cached. In your implementation, instantiate the appropriate template class and populate the resulting object with localized data. The data you supply should be fake, but it should reflect what your complication would normally look like.

If you pass `nil` to the handler, the system generates a default placeholder template from your app’s icon and name.

## See Also

### Related Documentation

class func localizableTextProvider(withStringsFileTextKey: String) -> Self

Creates a localizable simple text provider using the strings file key for the text.

Deprecated

class func localizableTextProvider(withStringsFileFormatKey: String, textProviders: [CLKTextProvider]) -> Self

Creates a localizable text provider with a strings file key that resolves to a format string, and with text providers for the replacement arguments.

Deprecated

class func localizableTextProvider(withStringsFileTextKey: String, shortTextKey: String?) -> Self

Creates a localizable simple text provider using strings file keys for both the regular text and the shorter fallback text.

Deprecated

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

