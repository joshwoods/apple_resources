

- tvOS Release Notes
-  tvOS 15.4 Release Notes 

Article

# tvOS 15.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The tvOS 15.4 SDK provides support to develop tvOS apps for Apple TV devices running tvOS 15.4. The SDK comes bundled with Xcode 13.3.1, available from the Mac App Store. For information on the compatibility requirements for Xcode 13.3.1, see Xcode 13.3.1 Release Notes.

### General

#### New Features

- Captive Wi-Fi network support on tvOS allows you to use your iPhone or iPad to connect your Apple TV to networks that need additional sign-in steps, like at hotels or dorms. (8351052)

### libc++

#### New Features

- The following new C++20 and C++23 features are now implemented:

  - C++20 library concepts defined in ``.

  - `constexpr` for `std::swap()` and swap-related functions.

  - Miscellaneous `constexpr`-ification in the library.

  - `std::atomic` now default initializes as expected.

  - A `.contains()` method for associative containers.

  - Added `std::bind_front()`. (88131816)

#### Deprecations

- Some extensions in `std::tuple` were removed to fix bugs caused by those extensions:

  - Tuples can no longer be constructed from fewer than the number of elements in the tuple. Previously, elements that weren’t specified were default-constructed; now this is a compiler error.

  - A tuple can no longer be constructed from an array.

  - The `std::result_of` and `std::is_literal_type` type traits are no longer available in C++20 mode, as specified in the Standard.

### StoreKit

#### New Features

- SKTestSession has three new methods to simulate a subscription requiring price increase consent, simulate consenting to a pending price increase, and simulate declining a price increase in automated tests. (84556183)

- `SKTestSession` has two new Boolean properties to simulate billing retry and grace period in automated tests. You can identify and simulate the resolution of billing retry issues using the same APIs as interrupted purchases. (83956205)

- Users can now test the billing retry and grace period states using StoreKit Testing in Xcode. Use Xcode 13.3 or later to enable billing retry testing and toggle whether the app offers a grace period. Use isInBillingRetry and gracePeriodExpirationDate to handle these states in the app. (83938270)

- You can now test offer codes with StoreKit Testing in Xcode. Configure offers for codes in Xcode 13.3 or later, and test redeeming them using presentCodeRedemptionSheet(). (63692551)

- Users can test subscription price increase behavior using StoreKit Testing in Xcode. Use Xcode 13.3 or later to set a price increase, then use paymentQueueShouldShowPriceConsent(_:), showPriceConsentIfNeeded(), and priceIncreaseStatus in the app. (58770817)

- `StoreKit` error types now conform to LocalizedError. (78735204)

- Some types in `StoreKit` now have a `localizedDescription` read-only `String` instance property. This property can be used to get a human-readable description of the value, localized for the device’s current locale. These types include: Product.ProductType, Product.SubscriptionInfo.RenewalState, expirationReason, priceIncreaseStatus, Transaction.OfferType, Product.SubscriptionOffer.OfferType, Product.SubscriptionOffer.PaymentMode, Product.SubscriptionPeriod.Unit, Transaction.RevocationReason, and Transaction.OwnershipType. (78735060)

- updates now emits unfinished transactions when iterating for the first time. (85294525)

- When using StoreKit Testing in Xcode, updates now emits all updated transactions. (85877689)

## See Also

### tvOS 15

tvOS 15.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 15.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 15.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 15.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 15.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 15 Release Notes

Update your apps to use new features, and test your apps against API changes.

