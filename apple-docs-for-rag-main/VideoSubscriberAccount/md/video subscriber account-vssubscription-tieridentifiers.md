

- Video Subscriber Account
- VSSubscription
-  tierIdentifiers 

Instance Property

# tierIdentifiers

A list of content from your catalog that the subscriber can access.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedmacOStvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var tierIdentifiers: [String]! { get set }
```

## Discussion

You should only use values that are in your availability feed’s tier restrictions.

## See Also

### Setting Subscription Details

var accessLevel: VSSubscriptionAccessLevel

The subscriber’s level of access to your catalog of content.

enum VSSubscriptionAccessLevel

Constants representing a subscriber’s level of access to your content.

var billingIdentifier: String?

The subscriber’s billing group.

var expirationDate: Date!

The date when the user’s subscription expires.

