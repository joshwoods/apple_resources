

- Video Subscriber Account
-  VSSubscriptionRegistrationCenter 

Class

# VSSubscriptionRegistrationCenter

An object that stores subscription information that the system provides to the Apple TV app.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedmacOStvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class VSSubscriptionRegistrationCenter
```

## Overview

Use the methods in this class to retrieve the default registration center object and set the user’s current subscription for your app. This subscription informs the Apple TV app of the user’s access level and tiers.

## Topics

### Setting the Current Subscription

func setCurrentSubscription(VSSubscription?)

Sets the subscription information for the current user.

### Getting the Default Registration Center

class func `default`() -> VSSubscriptionRegistrationCenter

Returns the default subscription registration center object.

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

class VSSubscription

An object that describes a subscriber’s access to content.

class VSAccountApplicationProvider

An object to display app-specific providers in your app.

