

- ClockKit
-  Deprecated articles and symbols 

API Collection

# Deprecated articles and symbols

## Topics

### Articles

Creating complications for your watchOS app

Set up and implement complications for your watchOS app.

Declaring complications for your app

Define the complications that your app supports.

Creating a timeline entry

Package your app-specific data into a template and create a timeline entry for that template.

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

### Other Symbols

class CLKComplicationServer

An object that manages the active complications for an app.

Deprecated

class CLKComplication

Metadata about a custom complication.

Deprecated

class CLKComplicationTimelineEntry

A container for the complication template object to display and the time to display it.

Deprecated

### Sample Code

Providing Multiple Complications

Present multiple complications for a single complication family using descriptors.

Creating and updating a complication’s timeline

Create complications that batch-load a timeline of future entries and run periodic background sessions to update the timeline.

### Templates

SwiftUI templates

Design complication templates using SwiftUI views.

enum ComplicationRenderingMode

The complication’s appearance, as specified by the watch face.

Deprecated

Data providers

Feed data to a complication template.

Circular small

Display small, circular content in the corners of the Color watch face.

Extra large

Display content on the X-Large watch face.

Modular small

Display content in the smaller spaces of the Modular watch face.

Modular large

Display multiple rows of content in the large, central complication on the Modular watch face.

Utilitarian

Use the utilitarian templates to display content on a variety of watch faces, including the Utility, Chronograph, Simple, and character watch faces.

Graphic

Display visually rich content on watch faces.

class CLKComplicationTemplate

An abstract class that defines the base behavior for all templates.

Deprecated

enum CLKComplicationFamily

Constants indicating the template groups.

Deprecated

CLKComplicationSupportedFamilies

The complication families for which the app can provide data.

Deprecated

