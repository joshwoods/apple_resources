

- ClockKit
- Deprecated articles and symbols
- Creating complications for your watchOS app
-  Adding Placeholders for Your Complication 

Article

# Adding Placeholders for Your Complication

Provide the placeholders that users see when adding your complication to a watch face.

## Overview

Create placeholders for all of the complication families that your app supports. Ideally, these placeholders should indicate the type of data that your complication usually shows. The system uses these placeholders to represent your complication when the user configures a watch face on Apple Watch.

You can provide placeholders in two ways: you can use static images for your placeholder, or dynamically create localized versions of the placeholders using complication templates. Ideally, your app provides both.

### Add Static Placeholder Images

When you first install your app, the system initially displays the static placeholders. The system then checks to see if your data source can generate a localized placeholder using a complication template. If the data source returns a valid template, the system transitions from the static image to the localized placeholder. The system then caches the template, and reuses the cached version until the user updates or reinstalls your app.

If you don’t provide any placeholders, the system generates a placeholder based on your app icon.

By default, when you create a new watchOS project, or add a watchOS target to an existing project, Xcode adds a Complication group to your WatchKit extension’s asset catalog.

Create PNG files to represent a complication for each family your app supports. Avoid using interlaced PNGs. Many complications use only the alpha channel of the image; however, graphic complications use full color images. For more information, see the Complications section of the Human Interface Guidelines.

Drag these files into the asset catalog, and drop them into the desired position. You can provide separate images for each screen size. If you don’t provide an image for a particular screen size, watchOS resizes the closest available image in that family.

### Create Localized Placeholders

To dynamically create a localized placeholder, implement your data source’s getLocalizableSampleTemplate(for:withHandler:) method. In your implementation, check the complication’s family, and create a template for that family. Populate the template with mock data that reflects what your complication would normally look like.

To localize the strings in your placeholder, use a simple text provider.

```
CLKSimpleTextProvider.localizableTextProvider(withStringsFileTextKey: "AKey")
```

The key must appear in a localized strings file named `ckcomplication.strings`. Save a copy of this strings file in your complication bundle and your WatchKit extension bundle. For more information, see Internationalization.

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

Enabling Complications for Your watchOS App

Set up your watchOS app’s complications.

