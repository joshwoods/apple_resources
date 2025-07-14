

- CarPlay
-  Supporting Previous Versions of iOS 

Article

# Supporting Previous Versions of iOS

Make your CarPlay-enabled apps compatible with older system versions, such as iOS 13 and earlier.

## Overview

In iOS 14 and later, CarPlay adds more app categories and further entitlements to support them. The framework also provides new templates that you can use to build your app’s user interface.

Some of the new app categories supersede existing ones, such as audio and communication. Using the proper combination of frameworks and entitlements, you can ensure that your app is compatible with iOS 13 and earlier, and iOS 14 and later. To learn about requesting entitlements for your CarPlay-enabled app, see Requesting CarPlay Entitlements.

### Add Backward Compatibility to Audio Apps

In iOS 14 and later, the CarPlay framework includes templates that you can use to build your audio app’s user interface. To use these templates, include the `com.apple.developer.carplay-audio` entitlement.

Before iOS 14, you built CarPlay-enabled audio apps using the Media Player framework, and included the `com.apple.developer.playable-content` entitlement. To support iOS 13 and earlier, use the Media Player framework and this entitlement. Your app will also work in iOS 14 and later.

Audio apps can use the CarPlay framework, the Media Player framework, or both. Include the applicable entitlements that match the frameworks you’re using. To be compatible with iOS 13 and earlier, as well as iOS 14 and later, specify keys for both entitlements in the entitlements file.

```
com.apple.developer.playable-content

com.apple.developer.carplay-audio

```

### Add Backward Compatibility to Communication Apps

In iOS 14 and later, the CarPlay framework includes templates that you can use to build your communication app’s user interface. To use these templates, include the `com.apple.developer.carplay-communication` entitlement.

Your communication app can use the CarPlay, SiriKit, or CallKit framework, or a combination of the three. Include the entitlements that match the frameworks you’re using. If you use the CarPlay framework, your app can’t present a custom user interface in iOS 13 or earlier. However, users can still interact with your app as they have in previous versions.

The following example shows what you might add to a messaging app’s entitlements file, providing compatibility with iOS 13 and earlier, as well as iOS 14 and later:

```
com.apple.developer.carplay-communication

com.apple.developer.carplay-messaging

```

If your CarPlay-enabled communication app includes VoIP features, provide support for doc://com.apple.documentation/documentation/sirikit/instartcallintent. If the VoIP app targets iOS 14 or earlier, provide support for doc://com.apple.documentation/documentation/sirikit/instartaudiocallintent and doc://com.apple.documentation/documentation/sirikit/insearchcallhistoryintent in addition to doc://com.apple.documentation/documentation/sirikit/instartcallintent.

## See Also

### CarPlay Integration

Requesting CarPlay Entitlements

Configure your CarPlay-enabled app with the entitlements it requires.

Displaying Content in CarPlay

Use scenes to present your app’s content on the vehicle’s built-in screen.

Using the CarPlay Simulator

Configure Simulator to run and debug your CarPlay-enabled app.

class CPTemplateApplicationScene

A CarPlay scene that controls your app’s user interface.

protocol CPTemplateApplicationSceneDelegate

The methods for responding to the life cycle events of your app’s scene.

class CPSessionConfiguration

An object that provides vehicle properties and configuration for the CarPlay environment.

