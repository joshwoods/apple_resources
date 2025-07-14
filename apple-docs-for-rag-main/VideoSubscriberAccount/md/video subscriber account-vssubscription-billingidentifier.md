

- Video Subscriber Account
- VSSubscription
-  billingIdentifier 

Instance Property

# billingIdentifier

The subscriber’s billing group.

iOS 11.3–18.0DeprecatediPadOS 11.3–18.0DeprecatedmacOStvOS 11.3–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var billingIdentifier: String? { get set }
```

## Discussion

You can use this property to restrict content availability based on the proximity of the billing address to a specific venue.

## See Also

### Setting Subscription Details

var accessLevel: VSSubscriptionAccessLevel

The subscriber’s level of access to your catalog of content.

enum VSSubscriptionAccessLevel

Constants representing a subscriber’s level of access to your content.

var expirationDate: Date!

The date when the user’s subscription expires.

var tierIdentifiers: [String]!

A list of content from your catalog that the subscriber can access.

