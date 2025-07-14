

- ClockKit
-  CLKComplicationDescriptor 

Class

# CLKComplicationDescriptor

A descriptor that defines a complication and the families that it supports.

watchOS 7.0+

``` source
class CLKComplicationDescriptor
```

## Mentioned in 

Declaring complications for your app

Creating a timeline entry

## Overview

Use complication descriptors to define the different types of complications that your app supports. Each descriptor provides a unique identifier for the complication, and the list of families that the complication supports. ClockKit defines the available families using the CLKComplicationFamily enumeration, while your app can define as many identifiers as it needs. Each unique identifier within your app represents a separate complication in the complication picker. For example, a weather app may have separate descriptors for `Condition`, `Temperature`, and `Precipitation.`

```
// Create the condition descriptor.
let conditionDescriptor = CLKComplicationDescriptor(
    identifier: complicationConditionIdentifier,
    displayName: "Weather Condition",
    supportedFamilies: mySupportedFamilies)

// Create the temperature descriptor.
let temperatureDescriptor = CLKComplicationDescriptor(
    identifier: complicationTemperatureIdentifier,
    displayName: "Temperature",
    supportedFamilies: mySupportedFamilies)

// Create the precipitation descriptor.
let precipitationDescriptor = CLKComplicationDescriptor(
    identifier: complicationPrecipitationIdentifier,
    displayName: "Percipitation",
    supportedFamilies: mySupportedFamilies)
```

You can dynamically create unique identifiers to further customize the complications. For example, if the weather app provides separate complications for all the cities in the user’s favorite city list, it can create a separate descriptor for each city and weather data pair. The app can create unique identifiers by appending the city name and the weather data’s name.

```
func getComplicationDescriptors(handler: @escaping ([CLKComplicationDescriptor]) -> Void) {
    var descriptors = [CLKComplicationDescriptor]()

    for city in myData.favoriteCities {

        let conditionIdentifier = complicationConditionIdentifier + ": \(city.id)"
        let temperatureIdentifier = complicationTemperatureIdentifier + ": \(city.id)"
        let perceptionIdentifier = complicationPrecipitationIdentifier + ": \(city.id)"

        // Create the descriptors for the city.
        descriptors.append(CLKComplicationDescriptor(
                            identifier: conditionIdentifier,
                            displayName: "\(city.abbreviation) Weather Condition",
                            supportedFamilies: CLKComplicationFamily.allCases,
                            userInfo: [myCityIDKey: city.id,
                                       myTypeIdentifierKey: conditionIdentifier]))

        descriptors.append(CLKComplicationDescriptor(
                            identifier: temperatureIdentifier,
                            displayName: "\(city.abbreviation) Temperature",
                            supportedFamilies: CLKComplicationFamily.allCases,
                            userInfo: [myCityIDKey: city.id,
                                       myTypeIdentifierKey: temperatureIdentifier]))

        descriptors.append(CLKComplicationDescriptor(
                            identifier: perceptionIdentifier,
                            displayName: "\(city.abbreviation) Percipitation",
                            supportedFamilies: CLKComplicationFamily.allCases,
                            userInfo: [myCityIDKey: city.id,
                                       myTypeIdentifierKey: perceptionIdentifier]))

    }

    // The order of the descriptors array
    // determines the order in the complication picker.
    handler(descriptors)
}
```

When dynamically creating identifiers, consider using the descriptor’s userInfo property to contain any additional information your app needs to create timeline entries for the complication. In the above example, the weather app adds the `myCityIDKey` and `myTypeIdentifierKey` `keys` so that it can access the city and weather data type without parsing the `identifier` string.

## Topics

### Creating descriptors

convenience init(identifier: String, displayName: String, supportedFamilies: [CLKComplicationFamily])

Returns a new complication descriptor.

Deprecated

convenience init(identifier: String, displayName: String, supportedFamilies: [CLKComplicationFamily], userActivity: NSUserActivity)

Returns a new complication descriptor with an associated user activity.

Deprecated

convenience init(identifier: String, displayName: String, supportedFamilies: [CLKComplicationFamily], userInfo: [AnyHashable : Any])

Returns a new complication descriptor with an associated dictionary of user data.

Deprecated

### Accessing the descriptor’s data

var identifier: String

A string that uniquely identifies the descriptor.

var displayName: String

A localized string that identifies complications from the descriptor to the user.

var supportedFamilies: [CLKComplicationFamily]

The families that support this type of complication.

var userActivity: NSUserActivity?

A user activity object that represents the state of the app at a moment in time.

var userInfo: [AnyHashable : Any]?

A dictionary of data that your data source can use to generate timeline entries.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Migration Support

Migrating ClockKit complications to WidgetKit

Leverage WidgetKit’s API to create watchOS complications using SwiftUI.

protocol CLKComplicationDataSource

A protocol that provides ClockKit with information about your complication.

let CLKDefaultComplicationIdentifier: String

An identifier representing a default complication.

