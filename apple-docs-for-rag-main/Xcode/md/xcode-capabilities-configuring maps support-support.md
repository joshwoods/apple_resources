

- Xcode
- Capabilities
-  Configuring Maps support 

Article

# Configuring Maps support

Register your iOS routing app to provide point-to-point directions to Maps and other apps.

## Overview

An iOS app that’s able to display point-to-point directions can register as a routing app and make those directions available to Maps along with all other apps on a user’s device. Registering as a routing app improves the user experience because other apps can access your app’s routing information, and these apps don’t need to provide their own routing directions. Because Maps displays apps in the App Store that provide directions, registering your iOS app as a routing app is a great way to let users know about it.

A routing app provides specific directions in addition to what Maps supports, such as subway routes, hiking trails, and bike paths. Before you can select the routing modes that your app supports, follow the steps in Add a capability to add the Maps capability to your app’s target.

Note

This capability is only applicable to custom routing apps on iOS. You don’t need to add the Maps capability to a macOS app to be able to use the MapKit framework.

### Select the supported routing modes

Before the system can distribute requests for directions to your routing app, you must inform it of the routing modes your app supports by following these  
steps:

1.  Select your project in Xcode’s Project navigator.

2.  Select the app’s target from the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Find the Maps capability.

5.  Select the relevant routing modes by checking the corresponding checkboxes.

Xcode adds the MKDirectionsApplicationSupportedModes array to your app’s `Info.plist` file (if not already present) and uses the modes you select to populate the array with the necessary values.

After you select the necessary routing modes, there are additional configuration steps you must complete before your app can start providing point-to-point directions, such as specifying a directions request document type and declaring your app’s geographic region. For more information, see Configuring Your App to Accept Direction Requests.

## See Also

### App execution

Configuring background execution modes

Indicate the background services your app requires to continue executing in the background in iOS, iPadOS, tvOS, visionOS, and watchOS.

Configuring custom fonts

Register your app as a provider or consumer of systemwide custom fonts.

Configuring game controllers

Enhance gameplay input by enabling the discovery, configuration, and use of physical game controllers.

Configuring Siri support

Enable your app and its Intents extension to resolve, confirm, and handle user-driven Siri requests for your app’s services.

