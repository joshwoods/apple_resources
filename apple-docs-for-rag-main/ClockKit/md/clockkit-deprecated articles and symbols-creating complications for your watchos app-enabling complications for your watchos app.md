

- ClockKit
- Deprecated articles and symbols
- Creating complications for your watchOS app
-  Enabling Complications for Your watchOS App 

Article

# Enabling Complications for Your watchOS App

Set up your watchOS app’s complications.

## Overview

Before adding complications to the Apple Watch face, you must enable support for them in your app. You can include the complications when you create a new app, or add complications to an existing app.

### Include Complications in a New App

Check Include Complications to enable complications when creating a new watchOS app, as shown in the figure below.

When you include complications, Xcode creates and configures a complication data source for your app. The data source includes stubs for many of the methods required to configure your complications, populate your timeline, and provide placeholders. Xcode also creates a group in your extension’s assets catalog for static placeholder images.

### Add Complications to an Existing App

To add complications to an existing watchOS app, you need to create these items yourself. Start by creating a class that adopts the CLKComplicationDataSource protocol.

```
import Foundation
import ClockKit

class ComplicationController: NSObject, CLKComplicationDataSource {

    func getCurrentTimelineEntry(for complication: CLKComplication, withHandler handler: @escaping (CLKComplicationTimelineEntry?) -> Void) {
        // TODO: Finish implementing this required method.
    }
}
```

Next, add a Complication group to your extension’s assets catalog (if one doesn’t already exist). Open the `Assets.xcassets` file and select Editor \> Add Assets \> watchOS \> New Watch Complication Placeholder, as in the figure below.

Finally, select your app in the Project navigator, and open the extension’s General tab. In the Complication Configuration set the Data Source Class and Complication Group to the class and asset catalog group you just created.

## See Also

### Related Documentation

Declaring complications for your app

Define the complications that your app supports.

Creating a timeline entry

Package your app-specific data into a template and create a timeline entry for that template.

Loading future timeline events

Preserve battery life and improve performance on the watch by providing a timeline with expected data and updates.

Keeping your complications up to date

Replace or extend the data in your complication’s timeline.

### Configure Complications

Adding Placeholders for Your Complication

Provide the placeholders that users see when adding your complication to a watch face.

