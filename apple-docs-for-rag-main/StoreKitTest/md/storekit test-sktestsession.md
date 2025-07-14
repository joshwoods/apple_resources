

- StoreKit Test
-  SKTestSession 

Class

# SKTestSession

The controls and environment configuration you use to test StoreKit transactions in Xcode.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class SKTestSession
```

## Overview

This class controls the settings that the server uses when it processes transactions. Run tests that reconfigure the environment serially, not concurrently, to avoid overwriting each other’s environment settings.

Note

There’s a single instance of the test environment. All `SKTestSession` instances control the same test environment.

The test environment creates an SKTestTransaction instance each time your test code calls any method of `SKTestSession` that affects in-app purchases, including:

- buyProduct(productIdentifier:)

- refundTransaction(identifier:)

- enableAutoRenewForTransaction(identifier:)

- disableAutoRenewForTransaction(identifier:)

- forceRenewalOfSubscription(productIdentifier:)

- expireSubscription(productIdentifier:)

- approveAskToBuyTransaction(identifier:)

- declineAskToBuyTransaction(identifier:)

- resolveIssueForTransaction(identifier:)

You can manage the transactions in the test environment. To get a list of all transactions in the test environment, call allTransactions(). To delete a single transaction, call deleteTransaction(identifier:). To delete all the transactions, call clearTransactions().

Before automating a test session with `SKTestSession`, you must create a StoreKit configuration file. For more information, see Setting up StoreKit Testing in Xcode and init(configurationFileNamed:). Set disableDialogs to `true` to run tests without showing test environment UI.

## Topics

### Initializing test sessions

convenience init(configurationFileNamed: String) throws

Initializes the test session with the provided configuration file that you include in your application’s bundle.

init(contentsOf: URL) throws

Initializes the test session with a configuration file you provide through a URL.

func resetToDefaultState()

Removes all property overrides and resets all test session settings to their default state.

### Configuring the test environment

var storefront: String

The three-letter code that represents the region associated with the App Store storefront.

var locale: Locale

The value that determines the localization metadata the test environment uses.

var disableDialogs: Bool

A Boolean value that determines whether the testing environment disables dialogs during automated testing.

### Managing transactions in the test environment

func allTransactions() -> [SKTestTransaction]

Gets a list of all transactions in the test environment.

func deleteTransaction(identifier: Int) throws

Deletes a specific transaction from the test environment.

func clearTransactions()

Removes all transactions from the test environment.

### Forcing failed transactions

var failTransactionsEnabled: Bool

A Boolean value that determines whether transactions fail in the testing environment.

Deprecated

var failureError: SKError.Code

The error code that transactions return when you enable failing transactions.

Deprecated

### Testing interrupted purchases

var interruptedPurchasesEnabled: Bool

A Boolean value that determines whether the test environment simulates an interrupted purchase.

func resolveIssueForTransaction(identifier: Int) throws

Simulates resolving an issue when you test interrupted purchases or billing retry scenarios.

### Testing Ask To Buy transactions

var askToBuyEnabled: Bool

A Boolean value that determines whether the testing environment simulates an Ask to Buy scenario.

func approveAskToBuyTransaction(identifier: Int) throws

Resolves an Ask to Buy test scenario by approving the transaction.

func declineAskToBuyTransaction(identifier: Int) throws

Resolves an Ask to Buy test scenario by declining the transaction.

### Testing subscription renewals

var timeRate: SKTestSession.TimeRate

The rate at which time passes for subscriptions in the test environment as compared to real time.

enum TimeRate

The values for rates of time passing in the test environment.

func enableAutoRenewForTransaction(identifier: Int) throws

Enables auto-renewing for an auto-renewable subscription in the test environment.

func disableAutoRenewForTransaction(identifier: Int) throws

Disables auto-renewing for an auto-renewable subscription in the test environment.

func forceRenewalOfSubscription(productIdentifier: String) throws

Ends the previous subscription period and begins the next period in the test environment.

func expireSubscription(productIdentifier: String) throws

Causes the identified auto-renewable subscription to expire immediately in the test environment.

### Testing billing retry and grace period

var billingGracePeriodIsEnabled: Bool

A Boolean value that indicates whether the test environment simulates a billing grace period for auto-renewable subscriptions.

var shouldEnterBillingRetryOnRenewal: Bool

A Boolean value that indicates whether the testing environment enters a billing retry state when an auto-renewable subscription renews.

func resolveIssueForTransaction(identifier: Int) throws

Simulates resolving an issue when you test interrupted purchases or billing retry scenarios.

### Testing price increase consent

func requestPriceIncreaseConsentForTransaction(identifier: Int) throws

Simulates a price increase that requires customer consent for an auto-renewable subscription.

func consentToPriceIncreaseForTransaction(identifier: Int) throws

Simulates a user consenting to a price increase for an auto-renewable subscription.

func declinePriceIncreaseForTransaction(identifier: Int) throws

Simulates a user canceling an auto-renewable subscription by disabling auto-renew.

### Testing externally performed transactions

func buyProduct(productIdentifier: String) throws

Simulates buying an in-app purchase or subscription outside the app.

Deprecated

func refundTransaction(identifier: Int) throws

Simulates a refund for an in-app purchase that completes outside of the app.

### Instance Methods

func buyProduct(identifier: Product.ID, options: Set&lt;Product.PurchaseOption>) async throws -> Transaction

func setSimulatedError&lt;API>(API.Failure?, forAPI: API) async throws

func simulatedError&lt;API>(forAPI: API) async -> API.Failure?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### StoreKit transaction testing

Setting up StoreKit Testing in Xcode

Prepare your test environment to test in-app purchases with data you configure locally.

class SKTestTransaction

A transaction that occurs in the testing environment.

