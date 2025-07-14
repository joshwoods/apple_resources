

- Safari Services
- Safari app extensions
- Safari app extension information property list keys
-  Using Safari app extension default keys 

Article

# Using Safari app extension default keys

Learn about the default keys in the information property list file.

## Overview

After you create a Safari app extension target in Xcode, you need to modify the information property list file, `Info.plist.` You make changes to identify your new Safari app extension, and specify its capabilities and access limits under the `NSExtension` key.

The keys under the `NSExtension` key apply to the Safari app extension point, `com.apple.Safari.extension` for macOS. Place these keys as subordinates of the `NSExtension` key.

A Safari app extension includes these entries by default:

`NSExtensionPointIdentifier`  
An identifier string to indicate a Safari extension: `com.apple.Safari.extension`.

`NSExtensionPrincipalClass`  
A string to indicate the class with the principal implementation for your extension, with a value of `SafariExtensionHandler`, which the `SafariExtensionHandler.swift` file defines in Swift, and the `SafariExtensionHandler.h` and `SafariExtensionHandler.m` files define in Objective-C.

`SFSafariContentScript`  
An array of dictionaries with a single entry, containing a `Script` key that specifies the `script.js` file in the template. When your extension loads, Safari automatically embeds this script file into every webpage that a user visits and the extension has access to. See Injecting a script into a webpage.

`SFSafariToolbarItem`  
A dictionary describing a toolbar item that uses the `ToolbarItemIcon.pdf` image from the template as the image for the button. See Adjusting settings for a toolbar item.

`SFSafariWebsiteAccess`  
A dictionary with two keys: the `Level` key to indicate the level of access (set to `Some`), and the `Allowed Domains` key, which includes an array of strings to limit the web addresses that your extension works with. For more information, see Adjusting website access permissions.

Although `SFSafariContentScript`, `SFSafariToolbarItem`, and `SFSafariWebsiteAccess` are all default keys, they’re not required because they specify features that may or may not exist in your Safari app extension. To learn more about feature keys, see Setting Safari app extension feature keys.

### Review the sample information property list

The code example below represents the overall structure of a typical `NSExtension` dictionary. Keep this structure in mind as you configure each element of your app extension.

```

   NSExtensionPointIdentifier
   com.apple.Safari.extension
   NSExtensionPrincipalClass
   SafariExtensionHandler
   SFSafariToolbarItem

       Action
       Command
       Identifier
       Button
       Image
       ToolbarItemIcon.pdf
       Label
       Your Button

   SFSafariContextMenu

           Text
           Search for selected text in MyApplication.
           Command
           Search

           Text
           Add an entry for selected text in MyApplication.
           Command
           Add

   SFSafariContentScript

           Script
           script.js

   SFSafariStyleSheet

           Style Sheet
           style.css

   SFSafariWebsiteAccess

       Allowed Domains

           *.webkit.org

       Level
       Some

```

