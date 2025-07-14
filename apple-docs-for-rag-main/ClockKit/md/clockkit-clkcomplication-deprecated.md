

- ClockKit
-  CLKComplication Deprecated

Class

# CLKComplication

Metadata about a custom complication.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplication
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

Sharing an Apple Watch face

## Overview

ClockKit defines each complication by its family and identifier properties. Each pair represents a unique complication that the user can select when configuring a watch face. When creating timeline entries, check both properties before creating and filling the complication’s template.

You specify the possible family and identifier combinations in your data source’s getComplicationDescriptors(handler:) method. Each of the CLKComplicationDescriptor objects you provide defines a unique identifier and the families that it supports.

In watchOS 6 and earlier, each app can have only one complication per supported family. When your app creates complication templates, determine the complication’s type from its family property only. For more information, see Declaring complications for your app.

You don’t create instances of this class directly. Instead, you retrieve them from the CLKComplicationServer object. Complication objects are only available when your complication is in use on the watch face.

In addition to getting information about the complication, you use complication objects to extend or replace the timeline data for one of your active complications. When calling the extendTimeline(for:) and reloadTimeline(for:) methods of the shared CLKComplicationServer object, pass the complication object you want to update.

## Topics

### Accessing Data About the Complication

var family: CLKComplicationFamily

The family to which the complication belongs.

var identifier: String

An identifier that specifies a complication if your app supports multiple complications per family.

var userActivity: NSUserActivity?

An object that represents the state of the app at a moment in time.

var userInfo: [AnyHashable : Any]?

A dictionary of additional data associated with the complication.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Other Symbols

class CLKComplicationServer

An object that manages the active complications for an app.

Deprecated

class CLKComplicationTimelineEntry

A container for the complication template object to display and the time to display it.

Deprecated

