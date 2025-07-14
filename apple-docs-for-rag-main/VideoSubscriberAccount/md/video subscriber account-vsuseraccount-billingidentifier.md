

- Video Subscriber Account
- VSUserAccount
-  billingIdentifier 

Instance Property

# billingIdentifier

A string that Identifies the billing group associated with the user account’s subscription.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS

``` source
var billingIdentifier: String? { get set }
```

## See Also

### User account information

var accountProviderIdentifier: String?

A string that uniquely identifies a provider known to Apple that provides the user account.

var accountType: VSUserAccount.AccountType

A constant that represents whether a user has access to paid content.

var authenticationData: String?

A string that represents an authentication token for the user account to authenticate with a provider.

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

