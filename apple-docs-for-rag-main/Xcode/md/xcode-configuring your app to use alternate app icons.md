

- Xcode
-  Configuring Your App to Use Alternate App Icons 

Sample Code

# Configuring Your App to Use Alternate App Icons

Add alternate app icons to your app, and let people choose which icon to display.

Download

iOS 15.0+iPadOS 15.0+Xcode 14.0+

## Overview

The sample code project demonstrates how to configure your app so that people can change the icon that appears on the Home screen, in Spotlight, and elsewhere in the system.

People select an alternate icon in the app interface from a collection that you provide.

### Add Icon Assets for the Alternate Icons

For each alternate app icon, the project requires multiple image files that vary in size. The project organizes these files through icon assets under the asset catalog.

The system picks the correct icon image for the current context and target device from the set of options under each icon asset. This ensures that the appearance of the alternate icon remains consistent.

For information on configuring app icons in the asset catalog, see Configuring your app icon.

For design guidance, see Human Interface Guidelines > App Icon.

### Configure the Asset Catalog Compiler

The system gathers information about the app’s icons from the app’s information property list file under the top-level key CFBundleIcons. Xcode adds entries to this file for the icons the project specifies through build settings under Asset Catalog Compiler - Options.

For each icon asset that the project specifies by name in the build setting Alternate App Icon Sets, Xcode adds an entry under the key CFBundleAlternateIcons.

Xcode enters the name of the primary app icon asset specified in the build setting Primary App Icon Set Name under the key CFBundlePrimaryIcon. This setting is also available through the App Icons and Launch Images section of the General pane.

For more information on build settings, see Build settings reference.

### Change the App’s Icon

When people select an alternate icon in the app interface, the app calls setAlternateIconName(_:completionHandler:) with the name of the new icon. This tells the system to display the new icon for this app. The system automatically displays an alert notifying people of the change. Passing `nil` displays the app’s primary icon.

UIApplication.shared.setAlternateIconName(iconName) { (error) in
    if let error = error {
        print(&quot;Failed request to update the app’s icon: \(error)&quot;)
    }
}

The current icon’s name is available through the property alternateIconName.

