

- Video Subscriber Account
-  VSUserAccount 

Structure

# VSUserAccount

An object that represents a user’s account.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS

``` source
struct VSUserAccount
```

## Overview

There are two sources for a `VSUserAccount` instance:

- You create an instance when a person registers a new account or signs into an existing account in your app, and you call update(_:) on VSUserAccountManager with the instance.

- You fetch user accounts by calling userAccounts(options:), which can return user accounts created on the current device, or user accounts registered on all the devices signed into the user’s iCloud account.

## Topics

### Creating user accounts

init(accountType: VSUserAccount.AccountType, updateURL: URL?)

Creates a user account object with a URL for account update requests.

enum AccountType

Constants that represent whether a user has access to paid content.

### User account information

var accountProviderIdentifier: String?

A string that uniquely identifies a provider known to Apple that provides the user account.

var accountType: VSUserAccount.AccountType

A constant that represents whether a user has access to paid content.

var authenticationData: String?

A string that represents an authentication token for the user account to authenticate with a provider.

var billingIdentifier: String?

A string that Identifies the billing group associated with the user account’s subscription.

var deviceCategory: VSUserAccount.OriginatingDeviceCategory

A constant that indicates whether the device from which the user registered is mobile.

enum OriginatingDeviceCategory

Constants that represent whether the device from which the user originally registered is mobile.

var identifier: String?

A string you provide that uniquely identifies the account.

var isFromCurrentDevice: Bool

A Boolean value that indicates whether the user originated their account on the current device.

var isSignedOut: Bool

A Boolean value that indicates whether the user has signed out of their account.

var requiresSystemTrust: Bool

A Boolean value that indicates whether the update URL must have a system-trusted certificate.

var subscriptionBillingCycleEndDate: Date?

A date that indicates when the billing cycle ends for a paid account.

var tierIdentifiers: [String]?

An array of strings that identify a subset of content from your catalog that the subscriber can play.

var updateURL: URL?

A URL that points to the application’s JavaScript endpoint for update requests.

### Instance Properties

var appleSubscription: VSAppleSubscription?

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### User account management

class VSUserAccountManager

The object that coordinates your app’s user account actions.

