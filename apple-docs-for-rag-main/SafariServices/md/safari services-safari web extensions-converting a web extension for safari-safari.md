

- Safari Services
- Safari web extensions
-  Converting a web extension for Safari 

Article

# Converting a web extension for Safari

Convert your existing extension to a Safari web extension using Xcode’s command-line tool.

## Overview

If you create a web extension that works in a browser other than Safari, you can deploy it in Safari by using the Safari web extension converter. The converter:

- Creates an Xcode project

- Configures the Xcode project with a macOS app or iOS app that installs the extension in Safari

- Configures a Safari web extension with your extension files in the Xcode project

### Run the converter

To run the converter, open the Terminal app and run the `xcrun` command with the `safari-web-extension-converter` option, providing the path for your existing extension files.

```
xcrun safari-web-extension-converter /path/to/extension
```

If the converter needs more information, it asks you interactively, or you can provide the following command-line options:

`--project-location`  
Save the generated app and Xcode project to the file path.

`--rebuild-project`  
Rebuild the existing Safari web extension Xcode project at the file path with different options or platforms. Use this option to add iOS to your existing macOS project.

`--app-name`  
Use the value to name the generated app and the Xcode project.

`--bundle-identifier`  
Use the value as the bundle identifier for the generated app. This identifier is unique to your app in your developer account. A reverse-DNS-style identifier is recommended (for example, `com.company.extensionName`).

`--swift`  
Use Swift in the generated app.

`--objc`  
Use Objective-C in the generated app.

`--ios-only`  
Create an iOS-only project.

`--macos-only`  
Create a macOS-only project.

`--copy-resources`  
Copy the extension files into the generated project. If you don’t specify this parameter, the project references the original extension files.

`--no-open`  
Don’t open the generated Xcode project when complete.

`--no-prompt`  
Don’t show the confirmation prompt.

`--force`  
Overwrite the output directory, if one exists.

`--help`  
Print the help text.

Important

By default, the converter creates a reference in the Xcode project to the resources in the path you provide. As a result, changes you make to the original extension update your converted Safari web extension and vice versa. If you prefer to keep your original and converted extensions separate, use the `--copy-resources` option to make a copy of the original files.

New Xcode projects require you to select either the Swift or Objective-C language for native development. For your Safari web extension, you may not need to make any native customizations at all because your extension uses the JavaScript, HTML, and CSS you provide. If you are unsure of which language to use, select Swift.

If the converter runs interactively, it asks you to confirm your selections and gives you the opportunity to update them.

### Review the manifest warnings

The converter generates and opens your new Xcode project. The converter reports any manifest keys that the current version of Safari doesn’t support.

```
Warning: The following keys in your manifest.json are not supported by your 
current version of Safari. If these are critical to your extension, you 
should review your code to see if you need to make changes to support Safari:
downloads
offline_enabled

```

Review any reported exceptions, and see Assessing your Safari web extension’s browser compatibility for details on how to resolve them.

### Build and run your converted Safari web extension

To see your converted extension in Safari, follow the instructions in Running your Safari web extension.

### Add iOS to your existing Xcode project

If you have an existing Xcode project with a macOS Safari web extension, and you want to add support for iOS to it, use the converter with the `--rebuild-project` option.

```
xcrun safari-web-extension-converter --rebuild-project /path/to/myExtension/myExtension.xcodeproj
```

Provide the path to your current extension’s Xcode project file (including the `xcodeproj` file extension). The converter creates a new Xcode project with both macOS and iOS extensions from your existing project, and prints manifest warnings.

## See Also

### Extension conversions

Converting a Safari app extension to a Safari web extension

Unify your web extensions and simplify development by sharing code with a Safari web extension.

