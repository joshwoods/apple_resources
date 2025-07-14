

- iOS &amp; iPadOS Release Notes
-  iOS & iPadOS 15.2 Release Notes 

Article

# iOS & iPadOS 15.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The iOS & iPadOS 15.2 SDK provides support to develop apps for iPhone, iPad, and iPod touch devices running iOS & iPadOS 15.2. The SDK comes bundled with Xcode 13.2, available from the Mac App Store. For information on the compatibility requirements for Xcode 13.2, see Xcode 13.2 Release Notes.

### App Privacy Report

#### New Features

- iOS & iPadOS 15 introduced the Record App Activity feature in the privacy settings, allowing people to save a summary of sensor, data, and internet access by apps on their device. In iOS & iPadOS 15.2, this activity is presented in Settings in a new UI called App Privacy Report. This is a great opportunity to review your app’s sensor, data, and internet usage. To view your activity in the report, go to Settings \> Privacy \> App Privacy Report \> Turn On App Privacy Report. Activity will show once you use your app. (78696668)

### App Store

#### New Features

- StoreKit APIs that present a refund request sheet can be tested with StoreKit Testing in Xcode. Use beginRefundRequest(in:) or beginRefundRequest(for:in:) when working with UIKit or the `refundRequestSheet(for:isPresented:onDismiss:)` view modifier when working with SwiftUI. (70794860)

- StoreKit APIs that present a sheet in your app to manage subscriptions can be tested with StoreKit Testing in Xcode. Use showManageSubscriptions(in:) when working with UIKit or the `manageSubscriptionsSheet(isPresented:)` view modifier when working with SwiftUI. (79975963)

- New SKTestSession.TimeRate values are available to use in automated tests with the StoreKit Test framework. (82680742)

#### Resolved Issues

- Subscriptions no longer continue to auto-renew after calling expireSubscription(productIdentifier:) in automated tests using StoreKit Test. (82800700)

- Pay-as-you-go offers are no longer displayed incorrectly in payment sheets when testing subscriptions with StoreKit Testing in Xcode. (74165210)

### Apple ID

#### New Features

- Legacy Contacts has been added to iOS & iPadOS 15.2, allowing users to designate people as legacy contacts for their accounts, as part of the Digital Legacy program. (84536375)

### iCloud Mail

#### New Features

- iCloud+ subscribers can now access and use Hide My Email directly from the Mail app. (84956894)

### Core Media

#### Known Issues

- Streaming in the Music app could result in higher CPU usage, causing faster battery drain in some scenarios. (84861891, 85326575)

### Location Emergency

#### New Features

- Auto Call can now be set up to use one of two methods for initiating an emergency call: holding the side button together with a volume button, or rapidly pressing the side button multiple times. Both methods now show a longer, 8-second countdown before placing an emergency call. (84620050)

### Reminders

#### New Features

- Tags can now be bulk renamed and deleted. (82177979)

### SwiftUI

#### Resolved Issues

- Using alert(_:isPresented:actions:message:) and doc://com.apple.documentation/documentation/swiftui/group/confirmationdialog(\_:ispresented:titlevisibility:actions:)-1v2e0 now present. (83731075)

- Pushing a ScrollView that has a background applied while inside of a stack style NavigationView when inside a TabView is now correctly tracked by the navigationBar and tabBar. (83686857)

- List correctly respects safe area insets. (83312573)

- Views are no longer hidden when using the iPad pointer to present a context menu. (83953549)

#### Known Issues

- A TextField won’t attempt to localize the raw string `TextField("Placeholder", text: $text)` when building against iOS 15 and running on older releases.

  **Workaround:** Wrap the string in a LocalizedStringKey. (82076857)

## See Also

### iOS &amp; iPadOS 15

iOS & iPadOS 15.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 15 Release Notes

Update your apps to use new features, and test your apps against API changes.

