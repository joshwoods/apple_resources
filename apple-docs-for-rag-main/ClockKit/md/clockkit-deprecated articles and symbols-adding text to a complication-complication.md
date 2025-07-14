

- ClockKit
- Deprecated articles and symbols
-  Adding text to a complication 

Article

# Adding text to a complication

Use text in SwiftUI complications.

## Overview

When creating ClockKit templates with SwiftUI views, Text views adapt their appearance based on the template’s complication family. The system automatically sets the font and size to match other templates in the same family.

### Match the Expected Font Size

Use the default font size as a guide for the type of information your complication displays. For example, the CLKComplicationTemplateGraphicExtraLargeCircularView template provides a large canvas for drawing, but it’s intended to present large, easy-to-read content instead of a lot of small, detailed data.

### Use Text Formatters

When displaying dates and times, use Text.DateStyle to create localized strings. Text.DateStyle also defines formatters such as relative, offset, and timer. ClockKit automatically updates information in these formatters, and you can use these formatters when instantiating a Text view.

```
Text(myEvent.startDate, style: .timer)
```

Or use them inline in an interpolated string.

```
Text("\(myEvent.name) starts in \(myEvent.startDate, style: .timer)")
```

## See Also

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

