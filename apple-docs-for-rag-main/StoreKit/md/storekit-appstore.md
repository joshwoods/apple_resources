

- StoreKit
-  AppStore 

Enumeration

# AppStore

Interactions with the App Store, such as managing subscriptions, verifying devices, authorizing payments, synchronizing transactions, getting the environment, and more.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum AppStore
```

## Overview

Use these static functions and variables to perform tasks like showing the manage subscriptions sheet, getting the device verification ID, determining whether users can make purchases, and more.

## Topics

### Checking the environment

struct Environment

Constants that represent the App Store server environment.

### Checking payment setup

static var canMakePayments: Bool

A Boolean value that indicates whether the person can make purchases.

### Verifying devices

static var deviceVerificationID: UUID?

The device verification identifier to use to verify whether signed information is valid for the current device.

### Getting the platform

struct Platform

Values that represent Apple platforms.

### Managing subscriptions

static func showManageSubscriptions(in: UIWindowScene) async throws

Presents the App Store sheet for managing subscriptions.

static func showManageSubscriptions(in: UIWindowScene, subscriptionGroupID: String) async throws

Presents the App Store sheet for managing subscriptions for a subscription group.

### Requesting reviews

struct RequestReviewAction

An instance that tells StoreKit to request an App Store rating or review, if appropriate.

static func requestReview(in: UIWindowScene)

Tells StoreKit to request an App Store rating or review from the user, if appropriate, using the specified scene.

static func requestReview(in: NSViewController)

Tells StoreKit to request an App Store rating or review from the user, if appropriate, using the specified view controller.

### Presenting the offer code redemption sheet

Supporting subscription offer codes in your app

Provide subscription service for customers who redeem offer codes through the App Store or within your app.

static func presentOfferCodeRedeemSheet(in: UIWindowScene) async throws

Displays a sheet in the window scene that enables users to redeem a subscription offer code that you configure in App Store Connect.

nonisolated func offerCodeRedemption(isPresented: Binding&lt;Bool>, onCompletion: @escaping @MainActor (Result&lt;Void, any Error>) -> Void = { _ in }) -> some View 

Presents a sheet that enables users to redeem subscription offer codes that you configure in App Store Connect.

static func presentOfferCodeRedeemSheet(from: NSViewController) async throws

Displays a sheet in the view that enables users to redeem a subscription offer code that you configure in App Store Connect.

### Restoring purchases

static func sync() async throws

Synchronizes your app’s transaction information and subscription status with information from the App Store.

## Relationships

### Conforms To

- Sendable

## See Also

### App Store interactions

struct AppTransaction

Information that represents the customer’s purchase of the app, cryptographically signed by the App Store.

