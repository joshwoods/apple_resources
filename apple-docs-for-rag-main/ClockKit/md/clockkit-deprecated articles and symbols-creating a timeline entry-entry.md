

- ClockKit
- Deprecated articles and symbols
-  Creating a timeline entry 

Article

# Creating a timeline entry

Package your app-specific data into a template and create a timeline entry for that template.

## Overview

ClockKit periodically requests timeline entries from your complication’s data source. A timeline entry consists of a complication template that you have configured with your app’s data and a date that specifies when ClockKit displays that template.

Your data source packages app-specific data into a template that ClockKit can display onscreen. To create the template, you examine the provided CLKComplication object, select an appropriate template, fill the template with data from your app, and then create a timeline entry for the template.

### Examine the Complication Object

When ClockKit requests a template, it always provides a CLKComplication object that describes the complication. The complication has an identifier that your app defines, and a family from the CLKComplicationFamily enumeration. Each identifier defines a separate complication type for the specified family.

Examine the identifier to determine which kind of complication you’re creating. In watchOS 7 and later, your app can provide one or more complications per family. For example, a weather app may support separate complications for the `Condition`, `Temperature`, and `Precipitation` identifiers.

```
switch complication.identifier {
case complicationConditionIdentifier:
    templateOrNil = myGetConditionTemplate(for: family, date: date)

case complicationTemperatureIdentifier:
    templateOrNil = myGetTemperatureTemplate(for: family, date: date)

case complicationPrecipitationIdentifier:
    templateOrNil = myGetPrecipitationPercentageTemplate(for: family, date: date)
```

The ClockKit framework organizes complications into families. Each family defines the size and shape of the complication. Examine the family to discover which kind of template you can use. For the complete list of families, see CLKComplicationFamily.

```
switch complication.family {
case .circularSmall:
    // Create a template from the circular small family.

case .modularSmall:
    // Create a template from the modular small family.

case .modularLarge:
    // Create a template from the modular large family.

// Continue with all the templates supported by the specified type.

@unknown default:
    print("*** Unknown Complication Family: \(complication.family) ***")
    // Handle the error here.
}
```

Each family provides one or more templates that define the type of data and the data’s position within the complication.

Select and create a template for the specified family from the following pages:

- Circular small

- Extra large

- Modular small

- Modular large

- Utilitarian

- Graphic

Note

For watchOS 6 and earlier, your app can provide only one complication per family. To support these versions of watchOS, you only need to check the complication’s family property when determining which template to use.

### Create Data Providers to Fill the Template

Data providers take a raw value and format it for the template. For example, the CLKSimpleTextProvider takes two strings—a short string and a long string. If you provide both, ClockKit selects the best string for the template’s size.

```
let temperature = myCity.temperature(date)

let nameProvider = CLKSimpleTextProvider(
    text: myCity.name,
    shortText: myCity.abbreviation)

let temperatureProvider = CLKSimpleTextProvider(
    text: "\(longNumberFormatter.string(from: NSNumber(value: temperature)) ?? "Unknown")º F",
    shortText: shortNumberFormatter.string(from: NSNumber(value: temperature)) ?? "??")
```

ClockKit uses data providers for text, images, and gauges, including:

- CLKSimpleTextProvider

- CLKDateTextProvider

- CLKTimeTextProvider

- CLKRelativeDateTextProvider

- CLKTimeIntervalTextProvider

- CLKImageProvider

- CLKFullColorImageProvider

- CLKSimpleGaugeProvider

- CLKTimeIntervalGaugeProvider

Some of the data providers, like CLKRelativeDateTextProvider and CLKTimeIntervalGaugeProvider, automatically update the complication as time passes without affecting your complication’s background execution budgets.

Use the data providers to create and populate your template.

```
let template = CLKComplicationTemplateModularSmallStackText(
    line1TextProvider: temperatureProvider,
    line2TextProvider: nameProvider)
```

### Use Complication Data

The CLKComplicationDescriptor class’s `userInfo` and `userActivity` properties let you pass additional data about the complication. You can use this data to simplify creating timeline entires, and to launch a particular scene in your app.

For example, you can create a set of complications from the user’s favorite city list, as shown in Dynamically Define Descriptors. Instead of parsing the complications identifier, you can add the city and the weather data type to the complication’s userInfo dictionary. Then, to create a timeline entry, you read the data from the dictionary before selecting and filling your template.

```
let city: City

// Read the city id from the complication's userInfo dictionary.
if let cityID = complication.userInfo?[myCityIDKey] as? String {
    city = myData.lookupCity(byID: cityID) ?? myData.currentCity
} else {
    city = myData.currentCity
}

let nameProvider = CLKSimpleTextProvider(
    text: city.name,
    shortText: city.abbreviation)

// Read the complication type from the userInfo dictionary.
let typeIdentifier = complication.userInfo?[myTypeIdentifierKey] as? String ?? "Undefined"
```

### Create the Timeline Entry Object

Create a CLKComplicationTimelineEntry object using the template and the desired date. For the current timeline entry, you must specify a date equal to or earlier than the current time.

```
CLKComplicationTimelineEntry(date: Date(), complicationTemplate: template)
```

For future timeline entries, specify the date and time for the data to appear on the complication. For a meeting complication, you might display information about a meeting before its scheduled start time. For more information on creating future timeline entries, see Loading future timeline events.

## See Also

### Related Documentation

Enabling Complications for Your watchOS App

Set up your watchOS app’s complications.

Adding Placeholders for Your Complication

Provide the placeholders that users see when adding your complication to a watch face.

### Articles

Creating complications for your watchOS app

Set up and implement complications for your watchOS app.

Declaring complications for your app

Define the complications that your app supports.

Loading future timeline events

Preserve battery life and improve performance on the watch by providing a timeline with expected data and updates.

Keeping your complications up to date

Replace or extend the data in your complication’s timeline.

Building complications with SwiftUI

Design the appearance of a graphic complication using SwiftUI.

Displaying progress views and gauges

Add rich visual data to your SwiftUI complications with progress views and gauges.

Adding text to a complication

Use text in SwiftUI complications.

