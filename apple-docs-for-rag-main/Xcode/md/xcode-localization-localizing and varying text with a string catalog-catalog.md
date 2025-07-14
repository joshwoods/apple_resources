

- Xcode
- Localization
-  Localizing and varying text with a string catalog 

Article

# Localizing and varying text with a string catalog

Use a string catalog to translate text, handle plurals, and vary the text your app displays on specific devices.

## Overview

Your app delivers the best experience when it runs well in a person’s locale and displays content in their native language. Supporting multiple languages is more than translating text. It includes handling plurals for nouns and units, as well as displaying the right form of text on specific devices.

Use a string catalog to localize and translate all your app’s text in a visual editor right in Xcode. A string catalog automatically tracks all the localizable strings from your code, and keeps your translations in one place.

Use string catalogs to host translations, configure pluralization messages for different regions and locales, and change how text appears on different devices.

Related session from WWDC23

Session 10155: Discover String Catalogs

### Localize your app’s text

Before you can translate text, you need to make it localizable. This involves wrapping the user-facing strings in your app in constructs that make them translatable.

In SwiftUI, all string literals within a view are automatically localizable.

```
// SwiftUI localizable text.
Text("Welcome")
```

Make general text localizable using the `String(localized:)` initializer. For apps targeting older platforms, use the `NSLocalizedString` macro.

```
// General localizable text.
String(localized: "Buy a book"))
```

Add comments to give context and assist localizers when translating your text.

```
// Localizable text with comments.
Text("Explore", comment: "The title of the tab bar item that navigates to the Explore screen.")
String(localized: "Get Started", comment: "The label on the Get Started button that appears after they sign in.")
```

### Add a string catalog to your project

To add a string catalog to your project, choose File \> New \> File.

In the sheet that appears, select the platform, enter `string` into the filter field, select String Catalog, and click Next. In the dialog that appears, accept the default name `Localizable`, choose a location, and click Create.

If your string catalog gets too big, you can create multiple string catalog files within a single Xcode project, and give each a unique name. Then choose which string catalog to use for each translation by passing the string catalog name to the `tableName` or `table` parameter to the respective localization API as follows:

```
// A SwiftUI localization example pointing to a specific string catalog.
Text("Explore", tableName: "Navigation")

// A general text localization example pointing to a specific string catalog.
String(localized: "Get Started", table: "MainScreen")
```

### Add a language to your project

To support multiple languages in your app, add additional languages to your project. For each language, select the string catalog in the Project navigator, click the Add button (+) near the bottom of the string catalog editor, and select a language to add.

### Add your localizable text to the string catalog

Xcode automatically keeps your string catalog and app in sync each time you build your project. To populate your string catalog with the localizable text from your app, choose Product \> Build. Xcode identifies strings in your app that support localization, and then adds them to your string catalog.

Use the percent symbol beside each language to track your string catalog’s percentage of translation.

### Add your translations using the string catalog editor

After identifying your localizable strings and adding them to a string catalog, you can either manually translate them, or you can export them, send them to a third-party for translation, and then import them.

To enter your app’s translations manually, select the string catalog and click the language you want to add translations for. Then click the text field of the Language column for each key in the table and enter the translation for that key.

Newly added strings that require translation appear with a New icon in the State column. When you add a translation, the New icon changes to a green checkmark. As you add translations, the percent symbol beside the language updates, displaying the translation percentage for that language. When a string catalog language reaches full translation, the percent symbol changes to a green checkmark.

For information about exporting and importing translations in Xcode, see Exporting localizations and Importing localizations.

### Add pluralizations

Languages have different grammatical rules for handling plurals of nouns and units. For example, in English, you can return `1 Book` when the value of `%lld` is `1`. And you can return `%lld Books` for all other cases. Other languages can have fewer or more plural variants, depending on their region and locale.

| Plural | Text         |
|--------|--------------|
| One    | `%lld Book`  |
| Other  | `%lld Books` |

To add a plural variant, first localize the text using the value the string is dependent on, using string interpolation.

```
@State private var itemCount = 0
Text("\(itemCount) Books")
```

Then, in the string catalog editor, select the language you want to add pluralization for, Control-click the variant key, and select the Vary by Plural option.

When you add a plural variant, the system does the following:

- Adds all the plural forms for that language into the string catalog editor.

- Determines which specifier to use for the interpolated string (`%lld` representing a 64-bit integer in this case).

- Prepopulates the variant fields with the value of that key.

Note

If you add pluralization to the source language (English in this case), the system propagates the variation to the other languages, if possible. If you add pluralization to a nonsource language, that change affects only that language.

Click the text field in the Language column for each variation of that string key, and enter the text for the system to use when that plural displays.

When you run the app, the pluralized variants update based on the value of the interpolated string.

### Vary strings by device

When you need to alter the text that displays on a device due to the available space, or because it has a different interaction, use the Vary by Device option in the string catalog editor.

For example, suppose you want to display two different messages depending on whether your app is running on iPhone or a Mac.

| Operating system | Message             |
|------------------|---------------------|
| iOS              | Tap to learn more   |
| macOS            | Click to learn more |

To vary the text string based on device, select the string catalog file, along with the language and key representing the message you want to vary. Control-click the key, select Vary by Device, and then select the device you want to add a specific message for.

Enter the text you want to display for that selected device, while retaining the existing text for all other devices. Add more devices if you need more variations.

When the app runs on the selected device, the system displays the new message for that device.

### Test your translations

To test your translations in the simulator:

1.  Change the app language of your current scheme by choosing Product \> Scheme \> Edit Scheme.

2.  In the dialog that appears, select the Run action on the left and click the Options tab.

3.  Click the App Language drop-down, select the language you want to test, and click Close.

You can also navigate to Settings on the simulated device and change the deviceʼs language there. When your app runs, the translations for the selected language appear in the simulator.

## See Also

### Essentials

Supporting multiple languages in your app

Internationalize your app’s strings, images, and other resource types to prepare for the translation process.

