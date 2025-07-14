

- Xcode
- Capabilities
-  Configuring custom fonts 

Article

# Configuring custom fonts

Register your app as a provider or consumer of systemwide custom fonts.

## Overview

In iOS 13 and later, your iOS app can contribute fonts for systemwide use and leverage fonts that other apps install.

When an app attempts the install one or more fonts systemwide, iOS prompts the user for their permission. If the user agrees, the installed fonts become accessible in Settings \> General \> Fonts. If your app provides installable fonts, include a UI that allows the user to browse those fonts and manage their registration.

You must store installable fonts in the app bundle or deliver them using On-Demand Resources, because the system prohibits an app from installing arbitrary fonts. Provide fonts in the TTF, OTF, or TTC formats or any of their modern variants, and package large font libraries as asset catalogs.

The system limits the number of installed fonts, and it derives that limit from the available system resources. If the user deletes your app, the system automatically removes any of the app’s installed fonts.

To register your app as a provider or consumer of systemwide custom fonts, follow the steps in Add a capability to add the Fonts capability to your app’s target.

Note

The Fonts capability is only available to use with iOS apps that target iOS 13 and later.

### Select the required privileges

Before your iOS app can install one or more custom fonts or use fonts that other apps provide, you must enable the necessary privileges by performing the following:

1.  Select your project in Xcode’s Project navigator.

2.  Select the iOS app’s target from the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Find the Fonts capability.

5.  Select the required privileges using the corresponding checkboxes.

Tip

Fonts privileges aren’t exclusive; your iOS app can provide fonts for use in other apps and consume fonts that other apps install systemwide.

Xcode adds the `com.apple.developer.user-fonts` array to your app’s entitlements file, if not already present, and uses the privileges you enable to populate that array with the corresponding values.

After enabling the required privileges, update your app to perform one or more of the following:

- Register fonts systemwide using one of these registration methods:

  - CTFontManagerRegisterFontURLs(_:_:_:_:)

  - CTFontManagerRegisterFontDescriptors(_:_:_:_:)

  - CTFontManagerRegisterFontsWithAssetNames(_:_:_:_:_:)

- Remove installed fonts using one of these unregister methods:

  - CTFontManagerUnregisterFontURLs(_:_:_:)

  - CTFontManagerUnregisterFontDescriptors(_:_:_:)

- Query all installed fonts using CTFontManagerRequestFonts(_:_:)

- Listen for font change notifications using kCTFontManagerRegisteredFontsChangedNotification

For more information, see the WWDC session video Font Management and Text Scaling.

## See Also

### App execution

Configuring background execution modes

Indicate the background services your app requires to continue executing in the background in iOS, iPadOS, tvOS, visionOS, and watchOS.

Configuring game controllers

Enhance gameplay input by enabling the discovery, configuration, and use of physical game controllers.

Configuring Maps support

Register your iOS routing app to provide point-to-point directions to Maps and other apps.

Configuring Siri support

Enable your app and its Intents extension to resolve, confirm, and handle user-driven Siri requests for your app’s services.

