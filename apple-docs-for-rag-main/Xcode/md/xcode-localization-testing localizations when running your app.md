

- Xcode
- Localization
-  Testing localizations when running your app 

Article

# Testing localizations when running your app

Run your app in each language and region you support to thoroughly test your app.

## Overview

After you import localizations that contain the translated strings and resources adapted for the culture and region, test each localization in your running app by choosing the language and region in the Run scheme. You can also automate testing of localizations using continuous integration by choosing a localization when you create a bot.

### Select a language and region in the scheme

In Xcode, choose Product \> Scheme \> Edit Scheme. In the sheet that appears, select the Run scheme action in the left column, and click Options on the right. Choose the language from the App Language pop-up menu and choose a region from the App Region pop-up menu:

| Region | Description |
|----|----|
| System Region | The operating system region settings. |
| \[Development Region\] | The region that you’re developing the app in (the second menu item). |
| \[Region\] | A specific region. Choose a region from a continent submenu. |

Click Close in the sheet and click the Run button in the toolbar.

### Choose the language and region for a bot

You can test the languages and regions you support systematically using continuous integration with a bot. In Xcode, from the Language and Region action pop-up menus in the bot configuration sheet, you can choose either a localization, pseudolanguage, or Use Scheme Settings. If you choose Use Scheme Settings from the Language menu, the bot uses the localization settings you choose from the App Language and App Region pop-up menus in the scheme editor.

Click Next in the sheet to complete the bot configuration.

For details on creating bots, see Continuous integration using Xcode Server in Xcode Help.

## See Also

### Testing

Previewing localizations

Test localizations in the SwiftUI preview or the Interface Builder preview.

