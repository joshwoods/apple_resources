

- Video Subscriber Account
- VSSubscription
-  expirationDate 

Instance Property

# expirationDate

The date when the user’s subscription expires.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedmacOStvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var expirationDate: Date! { get set }
```

## Discussion

This property defines the exact time when the subscription becomes inactive. When the current subscription becomes inactive, the system behaves as though the user isn’t a subscriber, similar to calling setCurrentSubscription(_:) with a value of `nil`.

You can use this property when a subscriber decides not to renew their subscription by setting an expiration date that corresponds to the final billing cycle end date.

You can also use this property when a subscription only grants access to time-limited content, such as a single season of games for a sports league.

The default is `distantFuture`.

## See Also

### Setting Subscription Details

var accessLevel: VSSubscriptionAccessLevel

The subscriber’s level of access to your catalog of content.

enum VSSubscriptionAccessLevel

Constants representing a subscriber’s level of access to your content.

var billingIdentifier: String?

The subscriber’s billing group.

var tierIdentifiers: [String]!

A list of content from your catalog that the subscriber can access.

