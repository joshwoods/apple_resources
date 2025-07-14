

- Safari Services
- Safari app extensions
- Safari app extension information property list keys
-  Setting Safari app extension feature keys 

Article

# Setting Safari app extension feature keys

Set keys for permissions, scripts, style sheets, contextual menu items, and toolbar items in the information property list file.

## Overview

After selecting which default keys to use in your Safari app extension’s information property list file, select the appropriate feature keys to identify files and UI items.

The table below lists the primary keys in the `NSExtension` dictionary that are associated with Safari app extension features. For information on available subkeys, see the link in the primary key description.

| Key | Type | Description |
|----|----|----|
| `SFSafariContentScript` | Array | An array for adding content scripts to the extension. Each value in the array is a dictionary that provides the filename for a content script.  For subkeys, see Using content script and style sheet keys. |
| `SFSafariContextMenu` | Array | An array for adding items to Safari’s context menu — the menu that appears when the user Control-clicks a webpage. For more information, see Adjusting settings for contextual menu items.  For subkeys, see Using contextual menu and toolbar item keys. |
| `SFSafariStyleSheet` | Array | An array for adding style sheets to the extension or to pages from a limited subset of URLs. Each value in the array is a dictionary that provides the filename for a content script.  For subkeys, see Using content script and style sheet keys. For more information, see Injecting CSS style sheets into a webpage. |
| `SFSafariToolbarItem` | Dictionary | A dictionary for adding a toolbar item to Safari windows.  For subkeys, see Using contextual menu and toolbar item keys. |
| `SFSafariWebsiteAccess` | Dictionary | An optional dictionary that specifies which webpages the Safari app extension can access, if any.  For details about configuring website access, see Adjusting website access permissions. |

In addition to the `NSExtension` keys, the `Info.plist` file includes an `NSHumanReadableDescription` key for your Safari app extension. When you install the app extension, the string value of this key appears in Safari \> Settings \> Preferences as the example below shows:

## See Also

### Access and permissions

Adjusting website access permissions

Set website access permissions in a Safari app extension using information property list keys.

Using permissions for scripts and style sheets

Learn about URL permissions for scripts and style sheets in a Safari app extension using information property list keys.

