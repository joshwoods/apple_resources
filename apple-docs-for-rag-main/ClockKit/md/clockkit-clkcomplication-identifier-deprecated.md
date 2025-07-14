

- ClockKit
- CLKComplication
-  identifier Deprecated

Instance Property

# identifier

An identifier that specifies a complication if your app supports multiple complications per family.

watchOS 7.0–9.0Deprecated

``` source
var identifier: String { get }
```

## Mentioned in 

Creating a timeline entry

## Discussion

In watchOS 7 and later, ClockKit represents a complication by its family and its CLKComplicationDescriptor. Descriptors often represent categories of information that the complication can display. For example, a weather app may support `Condition`, `Temperature`, and `Precipitation` descriptors.

```
let ComplicationConditionIdentifier = "ComplicationTypeCondition"
let ComplicationTemperatureIdentifier = "ComplicationTypeTemperature"
let ComplicationPrecipitationPercentageIdentifier = "ComplicationTypePrecipitationPercentage"
```

For apps created for watchOS 6 or earlier, the system automatically sets the configuration’s identifier property to CLKDefaultComplicationIdentifier if you don’t implement your data source’s getComplicationDescriptors(handler:) method. Similarly, the system sets the identifier to CLKDefaultComplicationIdentifier if the complication came from a shared watch face, but the sender chose to exclude private information.

Because default identifiers can come from shared watch faces, your data source’s getCurrentTimelineEntry(for:withHandler:) and getTimelineEntries(for:after:limit:withHandler:) methods must check for the CLKDefaultComplicationIdentifier value, and provide generic complication entries when it occurs.

## See Also

### Accessing Data About the Complication

var family: CLKComplicationFamily

The family to which the complication belongs.

Deprecated

var userActivity: NSUserActivity?

An object that represents the state of the app at a moment in time.

Deprecated

var userInfo: [AnyHashable : Any]?

A dictionary of additional data associated with the complication.

Deprecated

