

- Video Subscriber Account
-  VSSubscription 

Class

# VSSubscription

An object that describes a subscriber’s access to content.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedmacOStvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class VSSubscription
```

## Overview

Use a `VSSubscription` object to set user subscription information, such as account access type, proximity billing group, expiration date, and content catalog tier identifiers.

## Topics

### Setting Subscription Details

var accessLevel: VSSubscriptionAccessLevel

The subscriber’s level of access to your catalog of content.

enum VSSubscriptionAccessLevel

Constants representing a subscriber’s level of access to your content.

var billingIdentifier: String?

The subscriber’s billing group.

var expirationDate: Date!

The date when the user’s subscription expires.

var tierIdentifiers: [String]!

A list of content from your catalog that the subscriber can access.

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

## See Also

### TV app integration

class VSSubscriptionRegistrationCenter

An object that stores subscription information that the system provides to the Apple TV app.

class VSAccountApplicationProvider

An object to display app-specific providers in your app.

