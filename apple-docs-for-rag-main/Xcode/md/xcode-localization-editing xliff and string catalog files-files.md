

- Xcode
- Localization
-  Editing XLIFF and string catalog files 

Article

# Editing XLIFF and string catalog files

Translate or adapt the localizable files for a language and region that you export from your project.

## Overview

After you export localizations, you can give the Xcode Localization Catalog to localizers for translation, or edit the XLIFF files located in the `Localized Contents` folder yourself.

### Add translations to XLIFF files

To find the user-facing strings that need translation, including the app name, search for the `` element in the XLIFF file. To insert a translation of a string, add a `` element to the `` element containing the localized text as in:

```

        Hello, world!
        Hallo, Welt!
        A friendly greeting.

```

### Group related strings using tables

If you specify a table name when you internationalize your code — in other words, if you use the `Text` init(_:tableName:bundle:comment:) method or the NSLocalizedString(_:tableName:bundle:value:comment:) function with the `tableName` parameter — Xcode groups the strings into separate `` elements with `[table name].strings` as the filename. If you don’t specify a table name, Xcode uses the default `Localizable.strings` as the filename.

When you import the localizations, Xcode adds a version of the strings file for each localization to your project. In the following SwiftUI code listing, the first `Text` string appears in the default `Localized.strings` file while the Button label that specifies a table name appears in the `Buttons.strings` file:

```
VStack {
    Text("Hello, world!", comment:"A friendly greeting.")
        .font(.largeTitle)
        .padding()
    Button(action: pushMe){
        Text("Push Me", tableName:"Buttons", comment:"Push Me button label.")
    }
    .font(.title)
}
```

### Edit string catalogs in Xcode

After you import localizations, you can edit the string catalog file in your project and the next time you export localizations, Xcode includes your changes in the XLIFF files.

For more information about editing string catalogs in Xcode, see Localizing and varying text with a string catalog.

## See Also

### Translation and adaptation

Creating screenshots of your app for localizers

Share screenshots of your app with localizers to provide context for translation.

Exporting localizations

Provide the localizable files from your project to localizers.

Importing localizations

Import the files that you translate or adapt for a language and region into your project.

Locking views in storyboard and XIB files

Prevent changes to your Interface Builder files while localizing human-facing strings.

