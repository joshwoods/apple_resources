

- App Store Server API
-  SubscriptionGroupIdentifierItem 

Object

# SubscriptionGroupIdentifierItem

Information for auto-renewable subscriptions, including signed transaction information and signed renewal information, for one subscription group.

App Store Server API 1.0+

``` source
object SubscriptionGroupIdentifierItem
```

## Properties

`subscriptionGroupIdentifier`

subscriptionGroupIdentifier

The subscription group identifier of the auto-renewable subscriptions in the `lastTransactions` array.

`lastTransactions`

`[`lastTransactionsItem`]`

An array of the most recent App Store-signed transaction information and App Store-signed renewal information for all auto-renewable subscriptions in the subscription group.

## Topics

### Object and Data Types

subscriptionGroupIdentifier

object lastTransactionsItem

The most recent App Store-signed transaction information and App Store-signed renewal information for an auto-renewable subscription.

## See Also

### Response Objects and Data Types

type environment

The server environment, either sandbox or production.

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

