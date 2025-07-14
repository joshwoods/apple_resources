

- Video Subscriber Account
- VSSubscription
-  accessLevel 

Instance Property

# accessLevel

The subscriber’s level of access to your catalog of content.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedmacOStvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var accessLevel: VSSubscriptionAccessLevel { get set }
```

## Discussion

An error occurs if you try to set this property to VSSubscriptionAccessLevel.unknown.

## See Also

### Setting Subscription Details

enum VSSubscriptionAccessLevel

Constants representing a subscriber’s level of access to your content.

var billingIdentifier: String?

The subscriber’s billing group.

var expirationDate: Date!

The date when the user’s subscription expires.

var tierIdentifiers: [String]!

A list of content from your catalog that the subscriber can access.

