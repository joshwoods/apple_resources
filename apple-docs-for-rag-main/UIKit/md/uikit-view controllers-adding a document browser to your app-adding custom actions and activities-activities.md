

- UIKit
- View controllers
- Adding a document browser to your app
-  Adding custom actions and activities 

Article

# Adding custom actions and activities

Add custom document browser actions, activities, and bar items.

## Overview

There are three different ways to add custom actions to the document browser:

- Add document browser actions to the navigation bar or Edit Menu.

- Add activities to the activity view.

- Add bar items to the navigation bar.

### Add document browser actions

By default, the system provides a number of standard actions (copy, move, rename, delete, and share). To add custom actions, assign an array of UIDocumentBrowserAction objects to the browser’s customActions property.

Document browser actions can be accessed in two ways:

- *Navigation bar* actions appear in the navigation bar when the user places the browser into the Select mode.

- *Edit Menu* actions appear when the user long presses on a document or folder.

When triggered, these actions are passed the URLs of the currently selected items.

### Add activities

The browser displays an activity view when the user taps the Share button (for example, when the user long presses on a document or folder and selects Share from the Edit Menu).

To add custom activities to the activity view, implement your UIDocumentBrowserViewControllerDelegate object’s documentBrowser(_:applicationActivitiesForDocumentURLs:) method and return an array of custom UIActivity objects.

Your delegate object is passed an array of URLs for the currently selected items. You can store and use these URLs in your UIActivity subclass.

For more information, see Sharing and Actions.

### Add bar button items

Use the additionalLeadingNavigationBarButtonItems and additionalTrailingNavigationBarButtonItems methods to add buttons to the navigation bar.

Actions triggered by these buttons don’t have access to the browser’s content or to the URLs of selected items. Use bar button items for global actions only (actions that don’t affect a specific document or folder).

## See Also

### Customization

Customizing the browser

Customize the document browser’s look and behavior.

