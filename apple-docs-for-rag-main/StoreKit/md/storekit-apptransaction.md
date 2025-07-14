

- StoreKit
-  AppTransaction 

Structure

# AppTransaction

Information that represents the customer’s purchase of the app, cryptographically signed by the App Store.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AppTransaction
```

## Mentioned in 

Choosing a receipt validation technique

Validating receipts with the App Store

Supporting business model changes by using the app transaction

## Overview

Related sessions from WWDC22

Session 10007: What’s new with in-app purchase

## Topics

### Getting the signed app transaction

static var shared: VerificationResult&lt;AppTransaction>

Gets the App Store-signed app transaction information for the app.

### Getting the app transaction identifier

var appTransactionID: String

The unique identifier of the app download transaction.

### Getting the environment

let environment: AppStore.Environment

The server environment that signs the app transaction.

struct Environment

Constants that represent the App Store server environment.

### Getting app and version information

let bundleID: String

The bundle identifier that the app transaction applies to.

let appVersion: String

The app version that the app transaction applies to.

let originalAppVersion: String

The app version that the customer originally purchased from the App Store.

let appID: UInt64?

The unique identifier the App Store uses to identify the app.

let appVersionID: UInt64?

The number that the App Store uses to uniquely identify the version of the app.

### Getting the original platform

let originalPlatform: AppStore.Platform

The platform on which the customer originally purchased the app.

struct Platform

Values that represent Apple platforms.

### Getting purchase dates

let originalPurchaseDate: Date

The date the customer originally purchased the app from the App Store.

let preorderDate: Date?

The date the customer placed an order for the app before it’s available in the App Store.

### Verifying the app transaction

let deviceVerification: Data

The device verification value to use to verify whether the app transaction belongs to the device.

let deviceVerificationNonce: UUID

The UUID used to compute the device verification value.

let signedDate: Date

The date that the App Store signed the JWS app transaction.

### Getting app transaction information in JSON format

var jsonRepresentation: Data

The JSON representation of the app transaction information.

### Getting app transaction from the server

static func refresh() async throws -> VerificationResult&lt;AppTransaction>

Gets the App Store-signed app transaction information from the App Store server.

### Deprecated

var originalPlatformStringRepresentation: String

The string representation of the platform on which the customer originally purchased the app.

Deprecated

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### App transaction

Supporting business model changes by using the app transaction

Access the app transaction to learn when a customer first purchased an app, to determine the app features they’re entitled to.

