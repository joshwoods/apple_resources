

- macOS Release Notes
-  macOS Mojave 10.14.4 Release Notes 

Article

# macOS Mojave 10.14.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The macOS 10.14.4 SDK provides support for developing apps for Macs running macOS Mojave 10.14.4. The SDK comes bundled with Xcode 10.2 available from the Mac App Store. For information on the compatibility requirements for Xcode 10.2, see Xcode Release Notes.

### Accessibility

#### Known Issues

- VoiceOver may no longer be able to access web content when moving backward or forward through the current Safari tab’s history. (48831713)

  **Workaround:** In Safari, select Preferences \> Advanced \> “Show Develop menu in menu bar”, then deselect Develop \> Experimental Features \> “Swap Processes on Cross-Site Navigation”.

### App Store

#### Promoting Your Subscriptions with New Offers

StoreKit now supports subscription offers in addition to introductory offers, so apps with auto-renewable subscriptions can provide a discounted price for a specific duration for existing and previously subscribed customers. You can use subscription offers to help win back subscribers who have canceled their subscriptions or promote an upgrade to another subscription at a special price. Customers can accept the offer even if they’ve already completed an introductory offer.

StoreKit introduces a new array of SKProductDiscount objects within the SKProduct class to display offers within your app to eligible customers. Add a new SKPaymentDiscount object within the SKPayment class to allow these offers to be accepted by the customer.

### News

#### New Features

- Apple News is available in Canada with macOS 10.14.4. Apple News in Canada supports both English and French. Readers can access a bilingual experience when they follow a channel in a second language.

### Safari

#### Known Issues

- After updating to Safari 12.1 from Safari 10.1.2, web pages might not display. (47335741)

  **Workaround:** Run the following command in Terminal: `defaults delete com.apple.Safari`

  Warning

  You will lose your previous Safari settings after running the command above.

## See Also

### macOS 10.14

macOS Mojave 10.14.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Mojave 10.14.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Mojave 10.14.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Mojave 10.14.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Mojave 10.14 Release Notes

Update your apps to use new features, and test your apps against API changes.

