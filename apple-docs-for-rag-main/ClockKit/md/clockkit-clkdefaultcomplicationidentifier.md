

- ClockKit
-  CLKDefaultComplicationIdentifier 

Global Variable

# CLKDefaultComplicationIdentifier

An identifier representing a default complication.

watchOS 7.0+

``` source
let CLKDefaultComplicationIdentifier: String
```

## Discussion

The system assigns a CLKDefaultComplicationIdentifier value to the complication’s `identifier` property, whenever a specific identifier is unavailable. For example, ClockKit uses default type identifiers to represent the type on complications designed for watchOS 6 or earlier. It also uses the default type for complications from a shared watch face, when the sender chose to not include complication data in the shared watch face.

If your app supports multiple complications per family, you must check for CLKDefaultComplicationIdentifier values in your data source’s getCurrentTimelineEntry(for:withHandler:) and getTimelineEntries(for:after:limit:withHandler:) methods. If you receive a CLKDefaultComplicationIdentifier, return generic entries for the specified family.

```
switch complication.identifier {

case CLKDefaultComplicationIdentifier:
    templateOrNil = myGetConditionTemplate(for: complication, date: date)

case ComplicationTypeTemperatureIdentifier, CLKDefaultComplicationTypeIdentifier:
    templateOrNil = myGetTemperatureTemplate(for: complication, date: date)

case ComplicationTypePrecipitationPercentageIdentifier:
    templateOrNil = myGetPrecipitationPercentageTemplate(for: complication, date: date)

default:
    print("*** Unrecognized Complication Type ***")
    return nil
}
```

## See Also

### Migration Support

Migrating ClockKit complications to WidgetKit

Leverage WidgetKit’s API to create watchOS complications using SwiftUI.

protocol CLKComplicationDataSource

A protocol that provides ClockKit with information about your complication.

class CLKComplicationDescriptor

A descriptor that defines a complication and the families that it supports.

