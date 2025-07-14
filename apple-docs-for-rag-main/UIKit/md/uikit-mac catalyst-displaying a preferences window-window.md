

- UIKit
- Mac Catalyst
-  Displaying a Preferences window 

Article

# Displaying a Preferences window

Provide a Preferences window in your Mac app built with Mac Catalyst so users can manage app preferences defined in a Settings bundle.

## Overview

Mac apps typically display app-specific preferences using a Preferences window accessible through the standard Preferences menu item under the app menu in the menu bar.

Mac apps built with Mac Catalyst that include a `Settings.bundle` file automatically get the Preferences menu item and a Preferences window. When a user selects the Preferences menu item, the system displays a Mac-friendly Preferences window based on the options provided in your Settings bundle. To learn about Settings bundles, see Implementing an iOS Settings Bundle.

### Add a Preferences window to your app

To include a Preferences window in your Mac app, add a `Settings.bundle` file to your Xcode project by pressing Command-N and selecting the Settings Bundle template from the Resources section under iOS. Then click Next to save the file to your project.

### Add toolbar tabs to the Preferences window

A Settings bundle can include one or more child panes that allow you to organize your preferences hierarchically (see Hierarchical Preferences). In iOS, the Settings app displays a child pane as a preference row. When the user taps the row, the app displays a new view showing the preferences defined in the child pane’s property list file.

In macOS, the Preferences window displays a child pane as a tab on the window’s toolbar. When the user clicks the tab, they see the preferences provided in the child pane’s property list file.

The tab for a child pane displays the pane’s title and a system-provided icon. To customize the icon, add the following key to the child pane’s property list file:

`Icon`  
Optional. A string with the name of the image file to display as the toolbar tab icon in the Preferences window.

You must include the image file in the Settings bundle that contains the child pane’s property list file.

### Confirm changes made with a toggle switch

Another element of the Settings bundle is the Toggle Switch Element, which displays an ON/OFF switch that the user can toggle. Your Mac app can prompt the user for a confirmation when they toggle the switch by including the following keys in the toggle switch element:

`TrueConfirmationPrompt`  
Optional. A dictionary that defines the prompt to present to users when they attempt to turn on the switch.

`FalseConfirmationPrompt`  
Optional. A dictionary that defines the prompt to present to users when they attempt to turn off the switch.

Each dictionary contains the following keys that define the contents of the prompt:

`Type`  
Required. Must be set to `PSConfirmationPrompt`.

`Title`  
Required. A string with the title of the prompt. The title might not appear on some devices.

`Prompt`  
Required. A string with the body text that the prompt displays.

`ConfirmText`  
Optional. A string with the text displayed in the prompt’s confirmation button. The toggle switch value changes when the user clicks this button.

`DenyText`  
Optional. A string with the text displayed in the prompt’s cancel button. The toggle switch value doesn’t change when the user clicks this button.

### Display subtitles for toggle switches

Some iOS apps show descriptive text in a subtitle below a toggle switch using a group item with footer text. While the Preferences window supports this approach, the appearance on a Mac isn’t ideal. Instead, include the following key in the toggle switch element to show a subtitle:

`Description`  
Optional. A longer descriptive string to display under a toggle switch.

## See Also

### User preferences

Detecting changes in the preferences window

Listen for and respond to a user’s preference changes in your Mac app built with Mac Catalyst using Combine.

