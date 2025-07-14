

- Safari Services
- Safari app extensions
- Safari app extension information property list keys
-  Using contextual menu and toolbar item keys 

Article

# Using contextual menu and toolbar item keys

Learn about adding contextual menu items and toolbar items to a Safari app extension with information property list keys.

## Overview

Contextual menu items and toolbar items give you ways to add more menu options and entry points to your Safari app extension. You define and adjust these items using information property list keys.

### Add context menu items

The `SFSafariContextMenu` key lets your app extension add items to the context menu that appears in webpages. See Context menus for design guidelines.

The key’s value must be an array, and must contain one dictionary with two subkeys for each menu item.

| Subkey | Type | Description |
|----|----|----|
| `Text` | String | Required. A string that specifies the text to display for the context menu item. |
| `Command` | String | Required. A string that the context menu item sends when it activates. It contains the name of the command you want to send to your app extension when the user selects your item. |

For example, if you add two contextual menu items, your `Info.plist` file might look like the following:

```
SFSafariContextMenu

       Text
       Search for selected text in MyApplication.
       Command
       Search

       Text
       Add an entry for selected text in MyApplication.
       Command
       Add

```

### Add a toolbar item

The `SFSafariToolbarItem` dictionary adds a toolbar item to Safari windows. See Toolbars for design guidelines.

Each app extension can have only one toolbar item. The value for this key is a dictionary that describes the toolbar item. There are four required keys for the toolbar item dictionary.

| Subkey | Type | Description |
|----|----|----|
| `Identifier` | String | Required. A string identifier for the toolbar item. This doesn’t display to the user. |
| `Label` | String | Required. A string that appears in the overflow menu, in the Customize palette, and on hover. |
| `Image` | String | Required. A string specifying the filename of a scalable PDF image. The image must be transparent. Add the image file to your extension’s Xcode target. |
| `Action` | String | Required. A string specifying the command to send when the user clicks the toolbar item. Available actions are `Command` (to send a command to the app extension) and `Popover` (to display a popover window). This action determines which methods you need to implement to handle button events. |

Here’s an example dictionary in XML:

```

   Action
   Command
   Identifier
   Button
   Image
   Toolbar.pdf
   Label
   My Item

```

Use the `Image` key to provide an image for the toolbar button. Safari may resize or recolor the toolbar button image when drawing it to the screen. Make your image a template image and follow the guidelines for toolbar items.

Note

Buttons on the Safari toolbar are largely transparent, allowing them to fill with the appropriate gradient for the current macOS user interface. You don’t need to draw the button itself.

## See Also

### Contextual menu and toolbar items

Adjusting settings for a toolbar item

Customize a toolbar item for your Safari app extension.

Adjusting settings for contextual menu items

Customize contextual menu items for your Safari app extension.

class SFSafariToolbarItem

A proxy for a Safari app extension toolbar item in a Safari window.

class SFSafariExtensionViewController

The view controller for a popover associated with your app extension.

