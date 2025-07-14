

- Video Subscriber Account
-  VSSubscriptionAccessLevel 

Enumeration

# VSSubscriptionAccessLevel

Constants representing a subscriber’s level of access to your content.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedmacOStvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
enum VSSubscriptionAccessLevel
```

## Topics

### Subscription Tiers

case freeWithAccount

The user has access to free content with a valid account.

case paid

The user has access to content that requires a paid subscription.

case unknown

The default access level.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting Subscription Details

var accessLevel: VSSubscriptionAccessLevel

The subscriber’s level of access to your catalog of content.

var billingIdentifier: String?

The subscriber’s billing group.

var expirationDate: Date!

The date when the user’s subscription expires.

var tierIdentifiers: [String]!

A list of content from your catalog that the subscriber can access.

